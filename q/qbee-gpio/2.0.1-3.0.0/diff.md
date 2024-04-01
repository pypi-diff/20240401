# Comparing `tmp/qbee_gpio-2.0.1.tar.gz` & `tmp/qbee_gpio-3.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qbee_gpio-2.0.1.tar", max compression
+gzip compressed data, was "qbee_gpio-3.0.0.tar", max compression
```

## Comparing `qbee_gpio-2.0.1.tar` & `qbee_gpio-3.0.0.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0     1070 2024-03-11 09:52:06.863233 qbee_gpio-2.0.1/LICENSE
--rw-r--r--   0        0        0     5082 2024-03-11 09:52:06.863233 qbee_gpio-2.0.1/README.md
--rw-r--r--   0        0        0     1119 2024-03-11 09:52:06.863233 qbee_gpio-2.0.1/pyproject.toml
--rw-r--r--   0        0        0      398 2024-03-11 09:52:06.863233 qbee_gpio-2.0.1/qbee_gpio/__init__.py
--rw-r--r--   0        0        0     2996 2024-03-11 09:52:06.863233 qbee_gpio-2.0.1/qbee_gpio/config.py
--rw-r--r--   0        0        0      180 2024-03-11 09:52:06.863233 qbee_gpio-2.0.1/qbee_gpio/gpio/__init__.py
--rw-r--r--   0        0        0     6284 2024-03-11 09:52:06.863233 qbee_gpio-2.0.1/qbee_gpio/gpio/lcd_display.py
--rw-r--r--   0        0        0      377 2024-03-11 09:52:06.863233 qbee_gpio-2.0.1/qbee_gpio/gpio/setup.py
--rw-r--r--   0        0        0      655 2024-03-11 09:52:06.863233 qbee_gpio-2.0.1/qbee_gpio/gpio/switch.py
--rw-r--r--   0        0        0      401 2024-03-11 09:52:06.863233 qbee_gpio-2.0.1/qbee_gpio/gpio/types.py
--rw-r--r--   0        0        0      192 2024-03-11 09:52:06.863233 qbee_gpio-2.0.1/qbee_gpio/metadata/__init__.py
--rw-r--r--   0        0        0      376 2024-03-11 09:52:06.863233 qbee_gpio-2.0.1/qbee_gpio/metadata/interface.py
--rw-r--r--   0        0        0     1674 2024-03-11 09:52:06.863233 qbee_gpio-2.0.1/qbee_gpio/metadata/librespot.py
--rw-r--r--   0        0        0      360 2024-03-11 09:52:06.863233 qbee_gpio-2.0.1/qbee_gpio/metadata/model.py
--rw-r--r--   0        0        0     2236 2024-03-11 09:52:06.863233 qbee_gpio-2.0.1/qbee_gpio/metadata/pipe_reader.py
--rw-r--r--   0        0        0     1894 2024-03-11 09:52:06.863233 qbee_gpio-2.0.1/qbee_gpio/metadata/shairport.py
--rw-r--r--   0        0        0     6840 2024-03-11 09:52:06.863233 qbee_gpio-2.0.1/qbee_gpio/orchestrator.py
--rw-r--r--   0        0        0        0 2024-03-11 09:52:06.863233 qbee_gpio-2.0.1/qbee_gpio/py.typed
--rw-r--r--   0        0        0     1279 2024-03-11 09:52:06.863233 qbee_gpio-2.0.1/qbee_gpio/sound_poller.py
--rw-r--r--   0        0        0     5978 1970-01-01 00:00:00.000000 qbee_gpio-2.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1070 2024-04-01 14:45:22.911257 qbee_gpio-3.0.0/LICENSE
+-rw-r--r--   0        0        0     1778 2024-04-01 14:45:22.911257 qbee_gpio-3.0.0/README.md
+-rw-r--r--   0        0        0     1142 2024-04-01 14:45:22.915257 qbee_gpio-3.0.0/pyproject.toml
+-rw-r--r--   0        0        0      398 2024-04-01 14:45:22.915257 qbee_gpio-3.0.0/qbee_gpio/__init__.py
+-rw-r--r--   0        0        0     2604 2024-04-01 14:45:22.915257 qbee_gpio-3.0.0/qbee_gpio/config.py
+-rw-r--r--   0        0        0      181 2024-04-01 14:45:22.915257 qbee_gpio-3.0.0/qbee_gpio/gpio/__init__.py
+-rw-r--r--   0        0        0     7907 2024-04-01 14:45:22.915257 qbee_gpio-3.0.0/qbee_gpio/gpio/lcd_display.py
+-rw-r--r--   0        0        0      377 2024-04-01 14:45:22.915257 qbee_gpio-3.0.0/qbee_gpio/gpio/setup.py
+-rw-r--r--   0        0        0      318 2024-04-01 14:45:22.915257 qbee_gpio-3.0.0/qbee_gpio/gpio/switch.py
+-rw-r--r--   0        0        0      401 2024-04-01 14:45:22.915257 qbee_gpio-3.0.0/qbee_gpio/gpio/types.py
+-rw-r--r--   0        0        0      192 2024-04-01 14:45:22.915257 qbee_gpio-3.0.0/qbee_gpio/metadata/__init__.py
+-rw-r--r--   0        0        0      376 2024-04-01 14:45:22.915257 qbee_gpio-3.0.0/qbee_gpio/metadata/interface.py
+-rw-r--r--   0        0        0     1674 2024-04-01 14:45:22.915257 qbee_gpio-3.0.0/qbee_gpio/metadata/librespot.py
+-rw-r--r--   0        0        0      360 2024-04-01 14:45:22.915257 qbee_gpio-3.0.0/qbee_gpio/metadata/model.py
+-rw-r--r--   0        0        0     2200 2024-04-01 14:45:22.915257 qbee_gpio-3.0.0/qbee_gpio/metadata/pipe_reader.py
+-rw-r--r--   0        0        0     1894 2024-04-01 14:45:22.915257 qbee_gpio-3.0.0/qbee_gpio/metadata/shairport.py
+-rw-r--r--   0        0        0     5959 2024-04-01 14:45:22.915257 qbee_gpio-3.0.0/qbee_gpio/orchestrator.py
+-rw-r--r--   0        0        0        0 2024-04-01 14:45:22.915257 qbee_gpio-3.0.0/qbee_gpio/py.typed
+-rw-r--r--   0        0        0      760 2024-04-01 14:45:22.915257 qbee_gpio-3.0.0/qbee_gpio/sound_poller.py
+-rw-r--r--   0        0        0     2697 1970-01-01 00:00:00.000000 qbee_gpio-3.0.0/PKG-INFO
```

### Comparing `qbee_gpio-2.0.1/LICENSE` & `qbee_gpio-3.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `qbee_gpio-2.0.1/pyproject.toml` & `qbee_gpio-3.0.0/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,30 +1,30 @@
 [tool.poetry]
 name = "qbee-gpio"
-version = "2.0.1"
-description = "Control an LCD display and amplifier relay for use in an AirPlay Raspberry Pi server."
+version = "3.0.0"
+description = "Control an LCD display and amplifier relay for use in an AirPlay and/or Spotify Connect Raspberry Pi server."
 authors = ["Gabriel Pajot <gab@lescactus.eu>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/gpajot/qbee-gpio"
 include = ["qbee_gpio/py.typed"]
 
 [tool.poetry.dependencies]
 python = ">=3.8"
 
 asyncinotify = { version = ">=4.0,<4.1", python = "<4" }
 concurrent-tasks = ">=1.7,<2"
 zenconfig = { version = ">=2.1.0,<3", extras = ["yaml", "attrs"] }
 
 [tool.poetry.group.test.dependencies]
-pytest = "==8.0.2"
-pytest-asyncio = "==0.23.5"
-pytest-mock = "==3.12.0"
-ruff = "==0.3.2"
-mypy = "==1.8.0"
+pytest = "==8.1.1"
+pytest-asyncio = "==0.23.6"
+pytest-mock = "==3.14.0"
+ruff = "==0.3.4"
+mypy = "==1.9.0"
 pre-commit = "==3.5.0"
 
 [tool.poetry.scripts]
 qbee = 'qbee_gpio:run'
 
 [build-system]
 requires = ["poetry-core"]
```

### Comparing `qbee_gpio-2.0.1/qbee_gpio/config.py` & `qbee_gpio-3.0.0/qbee_gpio/config.py`

 * *Files 13% similar despite different names*

```diff
@@ -10,21 +10,20 @@
 class LCDConfig:
     # Change this to `False` to disable LCD.
     enable: bool = True
     # Size.
     width: int = 16
     lines: Literal[1, 2, 4] = 2
     # GPIO PIN configuration (BCM mode).
-    pin_power: int = 17
-    pin_register_select: int = 27
-    pin_enable: int = 18
-    pin_data_4: int = 25
-    pin_data_5: int = 24
-    pin_data_6: int = 23
-    pin_data_7: int = 22
+    pin_register_select: int = 23
+    pin_enable: int = 24
+    pin_data_4: int = 4
+    pin_data_5: int = 25
+    pin_data_6: int = 17
+    pin_data_7: int = 18
     shairport_metadata_path: Optional[Path] = attrs.field(
         default=Path("/tmp/shairport-sync-metadata"),
         converter=lambda e: Path(e) if e else None,
     )
     librespot_metadata_path: Optional[Path] = attrs.field(
         default=Path("/tmp/librespot-metadata"),
         converter=lambda e: Path(e) if e else None,
@@ -37,29 +36,24 @@
     # Change this to `True` to disable sound detection.
     enable: bool = True
     # We'll watch OPEN and CLOSE_WRITE events to detect sound output.
     driver_path: Path = attrs.field(
         default=Path("/dev/snd/pcmC0D0p"),
         converter=Path,
     )
-    # Command to check if something is currently playing.
-    # We'll consider that something is playing if the command outputs something in stdout.
-    # The default command will work if:
-    #   - `$_USER_ $_HOST_ = (root) NOPASWD: /usr/bin/fuser` has been added to sudoers
-    #   - or the user is root
-    currently_in_use_command: Optional[str] = "sudo fuser /dev/snd/pcmC0D0p"
     # Number of seconds to keep amp on after sound has stopped.
     standby_duration: Optional[float] = 600
     # Change this as needed or set to None to disable shutdown after standby.
     # The `sudo shutdown -h now` command will work if:
-    #   - `$_USER_ $_HOST_ = (root) NOPASWD: /usr/sbin/shutdown` has been added to sudoers
+    #   - `$_USER_ ALL = (root) NOPASWD: /usr/sbin/shutdown` has been added to sudoers
     #   - or the user is root
     shutdown_command: Optional[str] = None
     # GPIO PIN configuration (BCM mode).
-    pin_amp_power: int = 4
+    pin_on: int = 27
+    pin_standby: int = 22
 
 
 @attrs.define
 class QbeeConfig(zenconfig.Config):
     PATH: ClassVar[str] = "~/.qbee.yaml"
 
     sound_detection: SoundDetectionConfig = SoundDetectionConfig()
```

### Comparing `qbee_gpio-2.0.1/qbee_gpio/gpio/lcd_display.py` & `qbee_gpio-3.0.0/qbee_gpio/gpio/lcd_display.py`

 * *Files 26% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 @dataclass
 class GPIOLCDDisplay(contextlib.AbstractAsyncContextManager):
     """Hitachi HD44780 LCD controller.
     High level function to display text on the LCD.
 
     For more information see:
     - Condensed version: https://en.wikipedia.org/wiki/Hitachi_HD44780_LCD_controller
-    - Datasheet: https://cdn-shop.adafruit.com/datasheets/HD44780.pdf#page=54
+    - Datasheet: https://cdn-shop.adafruit.com/datasheets/HD44780.pdf
     """
 
     # PIN setup.
     # You will have to set up board/BCM mode yourself and those numbers should reflect that choice.
     pin_register_select: int
     pin_enable: int
     pin_data_4: int
@@ -61,59 +61,71 @@
         async with self._lock:
             self._init = False
 
     async def init(self) -> None:
         async with self._lock:
             # Init LCD.
             GPIO.output(self.pin_register_select, False)
-            await asyncio.sleep(0.015)
+            # No need to wait here as if the PI is booted power is already high enough.
             # Send 3 times the same command to ensure 8-bit mode.
-            await self._send_4_bits(0, 0, 1, 1)
-            await asyncio.sleep(0.004)  # Wait a bit more here as per specs.
-            await self._send_4_bits(0, 0, 1, 1)
-            await self._send_4_bits(0, 0, 1, 1)
+            await self._send_command((0, 0, 1, 1))
+            await asyncio.sleep(0.01)  # Wait more than 4.1ms here as per specs.
+            await self._send_command((0, 0, 1, 1))
+            await asyncio.sleep(0.001)  # Wait more than 100µs here as per specs.
+            await self._send_command((0, 0, 1, 1))
             # Now switch to 4-bit.
-            await self._send_4_bits(0, 0, 1, 0)
+            await self._send_command((0, 0, 1, 0))
             # Function set.
-            await self._send_4_bits(0, 0, 1, 0)
-            await self._send_4_bits(
-                bool(self.lines > 1),
-                bool(self.line_height != 8),
-                0,
-                0,
+            await self._send_command(
+                (0, 0, 1, 0),
+                (
+                    bool(self.lines > 1),
+                    bool(self.line_height != 8),
+                    0,
+                    0,
+                ),
             )
             # Display on/off control.
-            await self._send_4_bits(0, 0, 0, 0)
-            await self._send_4_bits(
-                1,
-                1,  # Screen on.
-                0,  # Cursor off.
-                0,  # Cursor blink off.
+            await self._send_command(
+                (0, 0, 0, 0),
+                (
+                    1,
+                    1,  # Screen on.
+                    0,  # Cursor off.
+                    0,  # Cursor blink off.
+                ),
             )
+            # Clear display.
+            await self._send_command((0, 0, 0, 0), (0, 0, 0, 1))
             # Entry mode set.
-            await self._send_4_bits(0, 0, 0, 0)
-            await self._send_4_bits(
-                0,
-                1,
-                1,  # Cursor moves right.
-                0,  # Display does not shit.
+            await self._send_command(
+                (0, 0, 0, 0),
+                (
+                    0,
+                    1,
+                    1,  # Cursor moves right.
+                    0,  # Display does not shit.
+                ),
             )
             self._init = True
 
     async def display(
         self,
         message: str,
         *,
         # Wrap content to spread on all available lines.
         wrap: bool = False,
         # This should be a function that takes a string and the width of the display
         # as arguments and return a string whose length is the same as the display.
         align: Callable[[str, int], str] = str.ljust,
     ) -> None:
         """Display a message on the screen."""
+        if not message.strip():
+            await self._send_command((0, 0, 0, 0), (0, 0, 0, 1))
+            return
         lines = message.split("\n")
         if wrap:
             wrapped_lines = []
             for line in lines:
                 # Convert each line in multiple ones based on the display width.
                 wrapped_lines += [
                     line[i : i + self.width] for i in range(0, len(line), self.width)
@@ -131,57 +143,103 @@
         await self._print_lines(lines)
 
     async def _print_lines(self, lines: Sequence[str]) -> None:
         async with self._lock:
             if not self._init:
                 return
             for i, line in enumerate(lines):
-                await self._send_byte(0x80 + self._line_addresses[i])
+                await self._send_command(
+                    *get_bits(0x80 + self._line_addresses[i]),
+                )
                 for char in line:
-                    await self._send_byte(ord(char), True)
+                    await self._send_char(ord(char))
 
-    async def _send_byte(self, byte: int, is_char: bool = False) -> None:
+    async def _send_char(self, byte: int) -> None:
         """Send a single byte."""
-        # Set the mode (command / char).
-        GPIO.output(self.pin_register_select, is_char)
+        # Set the mode.
+        GPIO.output(self.pin_register_select, True)
         # Send bits 4-7 then 0-3.
-        await self._send_nibble(byte >> 4, is_char)
-        await self._send_nibble(byte, is_char)
+        for bits in get_bits(byte):
+            await self._send_4_bits(*bits)
 
-    async def _send_nibble(self, byte: int, is_char: bool = False) -> None:
-        await self._send_4_bits(
-            bool(byte & 0x08),
-            bool(byte & 0x04),
-            bool(byte & 0x02),
-            bool(byte & 0x01),
-            is_char,
-        )
+    async def _send_command(
+        self,
+        *high_and_low_bits: Tuple[Bit, Bit, Bit, Bit],
+    ) -> None:
+        GPIO.output(self.pin_register_select, False)
+        for bits in high_and_low_bits:
+            await self._send_4_bits(*bits)
+        if high_and_low_bits == ((0, 0, 0, 0), (0, 0, 0, 1)):
+            # Wait more than 1.52ms after clear command.
+            await asyncio.sleep(0.002)
+        else:
+            # Wait more than 37µs after other commands.
+            await asyncio.sleep(0.00005)
 
     async def _send_4_bits(
         self,
         bit3: Bit,
         bit2: Bit,
         bit1: Bit,
         bit0: Bit,
-        is_char: bool = False,
     ) -> None:
         GPIO.output(self.pin_data_4, bit0)
         GPIO.output(self.pin_data_5, bit1)
         GPIO.output(self.pin_data_6, bit2)
         GPIO.output(self.pin_data_7, bit3)
-        await self._enable(is_char)
+        await self._enable()
 
-    async def _enable(self, is_char: bool) -> None:
-        await asyncio.sleep(0.000001)
+    async def _enable(self) -> None:
         GPIO.output(self.pin_enable, True)
         await asyncio.sleep(0.000001)
         GPIO.output(self.pin_enable, False)
-        await asyncio.sleep(0.0001 if not is_char else 0.000001)
+
+
+def get_bits(
+    byte: int,
+) -> Tuple[Tuple[Bit, Bit, Bit, Bit], Tuple[Bit, Bit, Bit, Bit]]:
+    high_bits = byte >> 4
+    return (
+        (
+            bool(high_bits & 0x08),
+            bool(high_bits & 0x04),
+            bool(high_bits & 0x02),
+            bool(high_bits & 0x01),
+        ),
+        (
+            bool(byte & 0x08),
+            bool(byte & 0x04),
+            bool(byte & 0x02),
+            bool(byte & 0x01),
+        ),
+    )
 
 
 def remove_accents(text: str) -> str:
     """Remove accents from text."""
     return (
         unicodedata.normalize("NFKD", text)
         .encode("ASCII", "ignore")
         .decode("utf-8", "ignore")
     )
+
+
+async def debug():
+    GPIO.setmode(GPIO.BCM)
+    try:
+        lcd = GPIOLCDDisplay(
+            pin_register_select=int(input("pin register select: ")),
+            pin_enable=int(input("pin enable: ")),
+            pin_data_4=int(input("pin data 4: ")),
+            pin_data_5=int(input("pin data 5: ")),
+            pin_data_6=int(input("pin data 6: ")),
+            pin_data_7=int(input("pin data 7: ")),
+        )
+        async with lcd:
+            while True:
+                await lcd.display(input("message: "), align=str.center)
+    finally:
+        GPIO.cleanup()
+
+
+if __name__ == "__main__":
+    asyncio.run(debug())
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `qbee_gpio-2.0.1/qbee_gpio/metadata/librespot.py` & `qbee_gpio-3.0.0/qbee_gpio/metadata/librespot.py`

 * *Files identical despite different names*

### Comparing `qbee_gpio-2.0.1/qbee_gpio/metadata/pipe_reader.py` & `qbee_gpio-3.0.0/qbee_gpio/metadata/pipe_reader.py`

 * *Files 2% similar despite different names*

```diff
@@ -36,15 +36,14 @@
         )
 
     def _close_transport(self) -> None:
         if self._transport:
             self._transport.close()
 
     def data_received(self, data: bytes) -> None:
-        logger.debug(data.decode())
         self._received_data.put_nowait(data)
 
     def connection_lost(self, exc):
         # If no exception it means write end has closed.
         if exc:
             logger.warning("error received while reading %s: %r", self.path, exc)
         # Signal to reconnect.
```

### Comparing `qbee_gpio-2.0.1/qbee_gpio/metadata/shairport.py` & `qbee_gpio-3.0.0/qbee_gpio/metadata/shairport.py`

 * *Files identical despite different names*

### Comparing `qbee_gpio-2.0.1/qbee_gpio/orchestrator.py` & `qbee_gpio-3.0.0/qbee_gpio/orchestrator.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 import asyncio
 import contextlib
 import logging.config
-from typing import List, Optional
+from typing import List
 
 from concurrent_tasks import BackgroundTask, LoopExceptionHandler
 
 from qbee_gpio.config import QbeeConfig
-from qbee_gpio.gpio import GPIOLCDDisplay, GPIOSwitch
+from qbee_gpio.gpio import GPIOLCDDisplay, gpio_switch
 from qbee_gpio.metadata import (
     LibrespotNowPlayingPoller,
     NowPlayingPoller,
     ShairportNowPlayingPoller,
 )
 from qbee_gpio.sound_poller import SoundPoller
 
@@ -44,41 +44,38 @@
                 pin_data_7=self._cfg.lcd.pin_data_7,
                 width=self._cfg.lcd.width,
                 lines=self._cfg.lcd.lines,
             )
             if self._cfg.lcd.enable
             else None
         )
-        self._amp_switch = (
-            GPIOSwitch(self._cfg.sound_detection.pin_amp_power)
+        self._on_switch = (
+            gpio_switch(self._cfg.sound_detection.pin_on)
             if self._cfg.sound_detection.enable
             else None
         )
-        self._lcd_switch = (
-            GPIOSwitch(self._cfg.lcd.pin_power)
-            if self._cfg.sound_detection.enable and self._cfg.lcd
+        self._standby_switch = (
+            gpio_switch(self._cfg.sound_detection.pin_standby)
+            if self._cfg.sound_detection.enable
             else None
         )
         self._standby_task = (
             BackgroundTask(self._standby) if self._cfg.sound_detection.enable else None
         )
         self._sound_poller = (
             SoundPoller(
                 self._cfg.sound_detection.driver_path,
-                self._cfg.sound_detection.currently_in_use_command,
             )
             if self._cfg.sound_detection.enable
             else None
         )
 
-        self._lock = asyncio.Lock()
         self._poll_sound_task = (
             BackgroundTask(self._poll_sound) if self._sound_poller else None
         )
-        self._current_power_stack: Optional[contextlib.AsyncExitStack] = None
         self._poll_now_playing_tasks: List[BackgroundTask] = []
         if self._cfg.lcd.enable and self._cfg.lcd.shairport_metadata_path:
             self._poll_now_playing_tasks.append(
                 BackgroundTask(
                     self._poll_now_playing,
                     ShairportNowPlayingPoller(self._cfg.lcd.shairport_metadata_path),
                 )
@@ -86,25 +83,26 @@
         if self._cfg.lcd.enable and self._cfg.lcd.librespot_metadata_path:
             self._poll_now_playing_tasks.append(
                 BackgroundTask(
                     self._poll_now_playing,
                     LibrespotNowPlayingPoller(self._cfg.lcd.librespot_metadata_path),
                 )
             )
-        self._last_message = (
-            self._cfg.lcd.startup_message if self._cfg.lcd.enable else ""
-        )
+        self._last_message = self._cfg.lcd.startup_message
         self._stop_event = asyncio.Event()
 
     async def __aenter__(self):
+        self._switch(False)
+        self.callback(self._switch, False)
         if self._standby_task:
             self.enter_context(self._standby_task)
-        self.push_async_callback(self._safe_turn_off)
         if self._poll_sound_task:
             self.enter_context(self._poll_sound_task)
+        if self._lcd:
+            await self.enter_async_context(self._lcd)
         for task in self._poll_now_playing_tasks:
             self.enter_context(task)
         return self
 
     async def run(self) -> None:
         logger.debug("starting orchestrator...")
         async with LoopExceptionHandler(stop_func=self._stop):
@@ -122,62 +120,46 @@
     async def _poll_sound(self) -> None:
         assert self._sound_poller
         assert self._standby_task
         async for output in self._sound_poller.poll():
             if output:
                 logger.debug("cancelling standby mode")
                 self._standby_task.cancel()
-                await self._safe_turn_on()
+                self._switch(True)
+                await self._print(self._last_message)
             else:
-                # Clear the display.
-                if self._lcd:
-                    await self._print("")
+                await self._print("")  # Clear the display.
                 self._standby_task.create()
 
-    async def _safe_turn_on(self) -> None:
-        assert self._amp_switch
-        async with self._lock:
-            if self._current_power_stack:
-                if self._lcd:
-                    await self._print(self._last_message)
-                return
-            logger.debug("turning on amp")
-            stack = contextlib.AsyncExitStack()
-            stack.enter_context(self._amp_switch)
-            if self._lcd_switch and self._lcd:
-                logger.debug("turning on lcd")
-                stack.enter_context(self._lcd_switch)
-                await stack.enter_async_context(self._lcd)
-                await self._print(self._last_message)
-            self._current_power_stack = stack
-
-    async def _safe_turn_off(self) -> None:
-        async with self._lock:
-            if not self._current_power_stack:
-                return
-            logger.debug("turning off amp and lcd")
-            await self._current_power_stack.aclose()
-            self._current_power_stack = None
-
     async def _standby(self) -> None:
         assert self._cfg.sound_detection
         if self._cfg.sound_detection.standby_duration is not None:
             logger.debug("entering standby mode")
             await asyncio.sleep(self._cfg.sound_detection.standby_duration)
             logger.debug("exiting standby mode")
-            await self._safe_turn_off()
+            self._switch(False)
         if self._cfg.sound_detection.shutdown_command:
             logger.info("shutting down system...")
             await asyncio.create_subprocess_shell(
                 self._cfg.sound_detection.shutdown_command,
             )
 
     # LCD.
 
     async def _poll_now_playing(self, poller: NowPlayingPoller) -> None:
         async for event in poller.poll():
             self._last_message = event.display(self._cfg.lcd.lines)
             await self._print(self._last_message)
 
     async def _print(self, message: str) -> None:
-        assert self._lcd
+        if not self._lcd:
+            return
         await self._lcd.display(message, align=str.center)
+
+    # Switches.
+
+    def _switch(self, value: bool) -> None:
+        if not self._standby_switch or not self._on_switch:
+            return
+        logger.debug("turning %s", "on" if value else "off")
+        self._on_switch(value)
+        self._standby_switch(not value)
```

