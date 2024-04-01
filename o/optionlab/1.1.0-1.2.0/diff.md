# Comparing `tmp/optionlab-1.1.0.tar.gz` & `tmp/optionlab-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "optionlab-1.1.0.tar", max compression
+gzip compressed data, was "optionlab-1.2.0.tar", max compression
```

## Comparing `optionlab-1.1.0.tar` & `optionlab-1.2.0.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0    35149 2024-03-24 15:08:09.757375 optionlab-1.1.0/LICENSE
--rw-r--r--   0        0        0    12317 2024-03-24 15:08:09.757375 optionlab-1.1.0/README.md
--rw-r--r--   0        0        0     4301 2024-03-24 15:08:09.761375 optionlab-1.1.0/optionlab/__init__.py
--rw-r--r--   0        0        0     9801 2024-03-24 15:08:09.761375 optionlab-1.1.0/optionlab/black_scholes.py
--rw-r--r--   0        0        0    19321 2024-03-24 15:08:09.761375 optionlab-1.1.0/optionlab/engine.py
--rw-r--r--   0        0        0    12899 2024-03-24 15:08:09.761375 optionlab-1.1.0/optionlab/models.py
--rw-r--r--   0        0        0     4726 2024-03-24 15:08:09.761375 optionlab-1.1.0/optionlab/plot.py
--rw-r--r--   0        0        0    12392 2024-03-24 15:08:09.761375 optionlab-1.1.0/optionlab/support.py
--rw-r--r--   0        0        0     1148 2024-03-24 15:08:09.761375 optionlab-1.1.0/optionlab/utils.py
--rw-r--r--   0        0        0      533 2024-03-24 15:08:09.761375 optionlab-1.1.0/pyproject.toml
--rw-r--r--   0        0        0    12845 1970-01-01 00:00:00.000000 optionlab-1.1.0/PKG-INFO
+-rw-r--r--   0        0        0    35149 2024-04-01 13:01:42.950066 optionlab-1.2.0/LICENSE
+-rw-r--r--   0        0        0    12431 2024-04-01 13:01:42.950066 optionlab-1.2.0/README.md
+-rw-r--r--   0        0        0     4383 2024-04-01 13:01:42.954066 optionlab-1.2.0/optionlab/__init__.py
+-rw-r--r--   0        0        0     9801 2024-04-01 13:01:42.954066 optionlab-1.2.0/optionlab/black_scholes.py
+-rw-r--r--   0        0        0    16823 2024-04-01 13:01:42.954066 optionlab-1.2.0/optionlab/engine.py
+-rw-r--r--   0        0        0    14386 2024-04-01 13:01:42.954066 optionlab-1.2.0/optionlab/models.py
+-rw-r--r--   0        0        0     5075 2024-04-01 13:01:42.954066 optionlab-1.2.0/optionlab/plot.py
+-rw-r--r--   0        0        0    12392 2024-04-01 13:01:42.954066 optionlab-1.2.0/optionlab/support.py
+-rw-r--r--   0        0        0     2630 2024-04-01 13:01:42.954066 optionlab-1.2.0/optionlab/utils.py
+-rw-r--r--   0        0        0      533 2024-04-01 13:01:42.954066 optionlab-1.2.0/pyproject.toml
+-rw-r--r--   0        0        0    12959 1970-01-01 00:00:00.000000 optionlab-1.2.0/PKG-INFO
```

### Comparing `optionlab-1.1.0/LICENSE` & `optionlab-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `optionlab-1.1.0/README.md` & `optionlab-1.2.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -33,15 +33,15 @@
 ## Basic usage
 
 Usage examples for several strategies can be found in the **examples** directory.
 
 To evaluate an option strategy, an `Inputs` model needs to be created:
 
 ```python
-from optionlab.models import Inputs
+from optionlab import Inputs
 inputs = Inputs.model_validate(inputs_data)
 ```
 
 The input data passed to `model_validate` above needs to be of the following structure: 
 
 ---
 
@@ -170,39 +170,48 @@
   - It must be 'closed'. It is mandatory.
 
 - `prev_pos` : float
   - The total value of the position to be closed, which can be positive if it made a profit or negative if it is a loss. It is mandatory.
 
 ---
 
-For example, let's say we wanted to calculate the probability of profit for naked calls on Apple stocks with maturity on December 17, 2021. The strategy setup consisted of selling 100 175.00 strike calls for 1.15 each on November 22, 2021.
-
-The inputs object must be passed to the `StrategyEngine` object as follows:
+For example, let's say we wanted to calculate the probability of profit for naked calls on Apple stocks 
+with maturity on December 17, 2021. The strategy setup consisted of selling 100 175.00 strike 
+calls for 1.15 each on November 22, 2021.
 
 ```python
-from optionlab.engine import StrategyEngine
-
 inputs_data = {
     "stock_price": 164.04,
     "start_date": "2021-11-22",
     "target_date": "2021-12-17",
     "volatility": 0.272,
     "interest_rate": 0.0002,
     "min_stock": 120,
     "max_stock": 200,
     "strategy": [
         {"type": "call", "strike": 175.0, "premium": 1.15, "n": 100, "action": "sell"}
     ],
 }
-st = StrategyEngine(Inputs.model_validate(inputs_data))
 ```
 
-The calculations are performed by calling the *run()* method of the *StrategyEngine* object:
+The calculations can be run by using:
+
+```python
+from optionlab import run_strategy
+
+out = run_strategy(inputs_data)
+```
+
+Alternatively, the inputs object can be passed to the `StrategyEngine` object and the calculations are performed by calling 
+the `run` method of the `StrategyEngine` object:
 
 ```python
+from optionlab import StrategyEngine
+
+st = StrategyEngine(Inputs.model_validate(inputs_data))
 out = st.run()
 ```
 
 This method returns an `Outputs` object with the following structure:
 
 ---
```

### Comparing `optionlab-1.1.0/optionlab/__init__.py` & `optionlab-1.2.0/optionlab/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import typing
 
 
-VERSION = "1.1.0"
+VERSION = "1.2.0"
 
 
 if typing.TYPE_CHECKING:
     # import of virtually everything is supported via `__getattr__` below,
     # but we need them here for type checking and IDE support
     from .models import (
         Inputs,
@@ -31,15 +31,15 @@
         get_d1_d2,
         get_bs_info,
         get_vega,
         get_delta,
         get_gamma,
         get_theta,
     )
-    from .engine import StrategyEngine
+    from .engine import StrategyEngine, run_strategy
     from .plot import plot_pl
     from .support import (
         get_pl_profile,
         get_pl_profile_stock,
         get_pl_profile_bs,
         create_price_seq,
         create_price_samples,
@@ -62,14 +62,15 @@
     "Distribution",
     "Strategy",
     "StrategyType",
     "StockStrategy",
     "Country",
     "Action",
     # engine
+    "run_strategy",
     "StrategyEngine",
     # support
     "get_pl_profile",
     "get_pl_profile_stock",
     "get_pl_profile_bs",
     "create_price_seq",
     "create_price_samples",
@@ -105,14 +106,15 @@
     "Strategy": (__package__, ".models"),
     "StrategyType": (__package__, ".models"),
     "StockStrategy": (__package__, ".models"),
     "Country": (__package__, ".models"),
     "Action": (__package__, ".models"),
     # engine
     "StrategyEngine": (__package__, ".engine"),
+    "run_strategy": (__package__, ".engine"),
     # support
     "get_pl_profile": (__package__, ".support"),
     "get_pl_profile_stock": (__package__, ".support"),
     "get_pl_profile_bs": (__package__, ".support"),
     "create_price_seq": (__package__, ".support"),
     "create_price_samples": (__package__, ".support"),
     "get_profit_range": (__package__, ".support"),
```

### Comparing `optionlab-1.1.0/optionlab/black_scholes.py` & `optionlab-1.2.0/optionlab/black_scholes.py`

 * *Files identical despite different names*

### Comparing `optionlab-1.1.0/optionlab/models.py` & `optionlab-1.2.0/optionlab/models.py`

 * *Files 6% similar despite different names*

```diff
@@ -12,15 +12,14 @@
 Country = Literal[
     "US",
     "Canada",
     "Mexico",
     "Brazil",
     "China",
     "India",
-    "India",
     "South Korea",
     "Russia",
     "Japan",
     "UK",
     "France",
     "Germany",
     "Italy",
@@ -283,16 +282,59 @@
 
 class OptionInfo(BaseModel):
     price: float
     delta: float
     theta: float
 
 
+def init_empty_array() -> np.ndarray:
+    return np.array([])
+
+
+class EngineDataResults(BaseModel):
+    stock_price_array: np.ndarray
+    terminal_stock_prices: np.ndarray
+    profit: np.ndarray = Field(default_factory=init_empty_array)
+    profit_mc: np.ndarray = Field(default_factory=init_empty_array)
+    strategy_profit: np.ndarray = Field(default_factory=init_empty_array)
+    strategy_profit_mc: np.ndarray = Field(default_factory=init_empty_array)
+    strike: list[float] = []
+    premium: list[float] = []
+    n: list[int] = []
+    action: list[Action | Literal["n/a"]] = []
+    type: list[StrategyType] = []
+    model_config = ConfigDict(arbitrary_types_allowed=True)
+
+
+class EngineData(EngineDataResults):
+    inputs: Inputs
+    _previous_position: list[float] = []
+    _use_bs: list[bool] = []
+    _profit_ranges: list[Range] = []
+    _profit_target_range: list[Range] = []
+    _loss_limit_ranges: list[Range] = []
+    _days_to_maturity: list[int] = []
+    _days_in_year: int = 365
+    days_to_target: int = 30
+    implied_volatility: list[float | np.ndarray] = []
+    itm_probability: list[float] = []
+    delta: list[float] = []
+    gamma: list[float] = []
+    vega: list[float] = []
+    theta: list[float] = []
+    cost: list[float] = []
+    profit_probability: float = 0.0
+    project_target_probability: float = 0.0
+    loss_limit_probability: float = 0.0
+
+
 class Outputs(BaseModel):
     """
+    data: EngineDataResults
+        Further results calculated by the engine.
     probability_of_profit : float
         Probability of the strategy yielding at least $0.01.
     profit_ranges : list
         A list of minimum and maximum stock prices defining
         ranges in which the strategy makes at least $0.01.
     strategy_cost : float
         Total strategy cost.
@@ -329,14 +371,16 @@
         Average loss as calculated from Monte Carlo-created terminal
         stock prices for which the strategy ends in loss.
     probability_of_profit_from_mc : float, optional
         Probability of the strategy yielding at least $0.01 as calculated
         from Monte Carlo-created terminal stock prices.
     """
 
+    inputs: Inputs
+    data: EngineDataResults
     probability_of_profit: float
     profit_ranges: list[Range]
     per_leg_cost: list[float]
     strategy_cost: float
     minimum_return_in_the_domain: float
     maximum_return_in_the_domain: float
     implied_volatility: list[float]
```

### Comparing `optionlab-1.1.0/optionlab/plot.py` & `optionlab-1.2.0/optionlab/plot.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,33 +1,36 @@
 from __future__ import division
 from __future__ import print_function
 
 import matplotlib.pyplot as plt
 from matplotlib import rcParams
 from numpy import zeros, full
 
-from optionlab import StrategyEngine
+from optionlab.models import Outputs
 
 
-def plot_pl(st: StrategyEngine):
+def plot_pl(outputs: Outputs) -> None:
     """
     plot_pl -> displays the strategy's profit/loss profile diagram.
 
     Returns
     -------
     None.
     """
+    st = outputs.data
+    inputs = outputs.inputs
+
     if len(st.strategy_profit) == 0:
         raise RuntimeError(
             "Before plotting the profit/loss profile diagram, you must run a calculation!"
         )
 
     rcParams.update({"figure.autolayout": True})
 
-    zero_line = zeros(st.s.shape[0])
+    zero_line = zeros(st.stock_price_array.shape[0])
     strike_call_buy = []
     strike_put_buy = []
     zero_call_buy = []
     zero_put_buy = []
     strike_call_sell = []
     strike_put_sell = []
     zero_call_sell = []
@@ -35,18 +38,18 @@
     comment = "P/L profile diagram:\n--------------------\n"
     comment += "The vertical green dashed line corresponds to the position "
     comment += "of the stock's spot price. The right and left arrow "
     comment += "markers indicate the strike prices of calls and puts, "
     comment += "respectively, with blue representing long and red representing "
     comment += "short positions."
 
-    plt.axvline(st.stock_price, ls="--", color="green")
+    plt.axvline(inputs.stock_price, ls="--", color="green")
     plt.xlabel("Stock price")
     plt.ylabel("Profit/Loss")
-    plt.xlim(st.s.min(), st.s.max())
+    plt.xlim(st.stock_price_array.min(), st.stock_price_array.max())
 
     for i, strike in enumerate(st.strike):
         if strike == 0.0:
             continue
 
         if st.type[i] == "call":
             if st.action[i] == "buy":
@@ -60,37 +63,37 @@
                 strike_put_buy.append(strike)
                 zero_put_buy.append(0.0)
             elif st.action[i] == "sell":
                 strike_put_sell.append(strike)
                 zero_put_sell.append(0.0)
 
     target_line = None
-    if st.profit_target is not None:
+    if inputs.profit_target is not None:
         comment += " The blue dashed line represents the profit target level."
-        target_line = full(st.s.shape[0], st.profit_target)
+        target_line = full(st.stock_price_array.shape[0], inputs.profit_target)
 
     loss_line = None
-    if st.loss_limit is not None:
+    if inputs.loss_limit is not None:
         comment += " The red dashed line represents the loss limit level."
-        loss_line = full(st.s.shape[0], st.loss_limit)
+        loss_line = full(st.stock_price_array.shape[0], inputs.loss_limit)
 
     print(comment)
 
     if loss_line is not None and target_line is not None:
         plt.plot(
-            st.s,
+            st.stock_price_array,
             zero_line,
             "m--",
-            st.s,
+            st.stock_price_array,
             loss_line,
             "r--",
-            st.s,
+            st.stock_price_array,
             target_line,
             "b--",
-            st.s,
+            st.stock_price_array,
             st.strategy_profit,
             "k-",
             strike_call_buy,
             zero_call_buy,
             "b>",
             strike_put_buy,
             zero_put_buy,
@@ -101,21 +104,21 @@
             strike_put_sell,
             zero_put_sell,
             "r<",
             markersize=10,
         )
     elif loss_line is not None:
         plt.plot(
-            st.s,
+            st.stock_price_array,
             zero_line,
             "m--",
-            st.s,
+            st.stock_price_array,
             loss_line,
             "r--",
-            st.s,
+            st.stock_price_array,
             st.strategy_profit,
             "k-",
             strike_call_buy,
             zero_call_buy,
             "b>",
             strike_put_buy,
             zero_put_buy,
@@ -126,21 +129,21 @@
             strike_put_sell,
             zero_put_sell,
             "r<",
             markersize=10,
         )
     elif target_line is not None:
         plt.plot(
-            st.s,
+            st.stock_price_array,
             zero_line,
             "m--",
-            st.s,
+            st.stock_price_array,
             target_line,
             "b--",
-            st.s,
+            st.stock_price_array,
             st.strategy_profit,
             "k-",
             strike_call_buy,
             zero_call_buy,
             "b>",
             strike_put_buy,
             zero_put_buy,
@@ -151,18 +154,18 @@
             strike_put_sell,
             zero_put_sell,
             "r<",
             markersize=10,
         )
     else:
         plt.plot(
-            st.s,
+            st.stock_price_array,
             zero_line,
             "m--",
-            st.s,
+            st.stock_price_array,
             st.strategy_profit,
             "k-",
             strike_call_buy,
             zero_call_buy,
             "b>",
             strike_put_buy,
             zero_put_buy,
```

### Comparing `optionlab-1.1.0/optionlab/support.py` & `optionlab-1.2.0/optionlab/support.py`

 * *Files identical despite different names*

### Comparing `optionlab-1.1.0/pyproject.toml` & `optionlab-1.2.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "optionlab"
-version = "1.1.0"
+version = "1.2.0"
 description = "Evaluate option strategies"
 authors = ["rgaveiga"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.10"
 scipy = "^1.12.0"
```

### Comparing `optionlab-1.1.0/PKG-INFO` & `optionlab-1.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: optionlab
-Version: 1.1.0
+Version: 1.2.0
 Summary: Evaluate option strategies
 Author: rgaveiga
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: holidays (>=0.44,<0.45)
@@ -49,15 +49,15 @@
 ## Basic usage
 
 Usage examples for several strategies can be found in the **examples** directory.
 
 To evaluate an option strategy, an `Inputs` model needs to be created:
 
 ```python
-from optionlab.models import Inputs
+from optionlab import Inputs
 inputs = Inputs.model_validate(inputs_data)
 ```
 
 The input data passed to `model_validate` above needs to be of the following structure: 
 
 ---
 
@@ -186,39 +186,48 @@
   - It must be 'closed'. It is mandatory.
 
 - `prev_pos` : float
   - The total value of the position to be closed, which can be positive if it made a profit or negative if it is a loss. It is mandatory.
 
 ---
 
-For example, let's say we wanted to calculate the probability of profit for naked calls on Apple stocks with maturity on December 17, 2021. The strategy setup consisted of selling 100 175.00 strike calls for 1.15 each on November 22, 2021.
-
-The inputs object must be passed to the `StrategyEngine` object as follows:
+For example, let's say we wanted to calculate the probability of profit for naked calls on Apple stocks 
+with maturity on December 17, 2021. The strategy setup consisted of selling 100 175.00 strike 
+calls for 1.15 each on November 22, 2021.
 
 ```python
-from optionlab.engine import StrategyEngine
-
 inputs_data = {
     "stock_price": 164.04,
     "start_date": "2021-11-22",
     "target_date": "2021-12-17",
     "volatility": 0.272,
     "interest_rate": 0.0002,
     "min_stock": 120,
     "max_stock": 200,
     "strategy": [
         {"type": "call", "strike": 175.0, "premium": 1.15, "n": 100, "action": "sell"}
     ],
 }
-st = StrategyEngine(Inputs.model_validate(inputs_data))
 ```
 
-The calculations are performed by calling the *run()* method of the *StrategyEngine* object:
+The calculations can be run by using:
+
+```python
+from optionlab import run_strategy
+
+out = run_strategy(inputs_data)
+```
+
+Alternatively, the inputs object can be passed to the `StrategyEngine` object and the calculations are performed by calling 
+the `run` method of the `StrategyEngine` object:
 
 ```python
+from optionlab import StrategyEngine
+
+st = StrategyEngine(Inputs.model_validate(inputs_data))
 out = st.run()
 ```
 
 This method returns an `Outputs` object with the following structure:
 
 ---
```

