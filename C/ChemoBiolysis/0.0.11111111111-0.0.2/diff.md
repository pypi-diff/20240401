# Comparing `tmp/ChemoBiolysis-0.0.11111111111.tar.gz` & `tmp/ChemoBiolysis-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ChemoBiolysis-0.0.11111111111.tar", last modified: Thu Mar 14 19:48:07 2024, max compression
+gzip compressed data, was "ChemoBiolysis-0.0.2.tar", last modified: Mon Apr  1 13:32:53 2024, max compression
```

## Comparing `ChemoBiolysis-0.0.11111111111.tar` & `ChemoBiolysis-0.0.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2024-03-14 19:48:07.915768 ChemoBiolysis-0.0.11111111111/
--rw-rw-rw-   0        0        0       84 2023-12-14 04:42:20.000000 ChemoBiolysis-0.0.11111111111/CHANGELOG.txt
-drwxrwxrwx   0        0        0        0 2024-03-14 19:48:07.846903 ChemoBiolysis-0.0.11111111111/ChemoBiolysis/
--rw-rw-rw-   0        0        0    65128 2024-03-14 13:59:45.000000 ChemoBiolysis-0.0.11111111111/ChemoBiolysis/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-14 19:48:07.911690 ChemoBiolysis-0.0.11111111111/ChemoBiolysis.egg-info/
--rw-rw-rw-   0        0        0     2768 2024-03-14 19:48:07.000000 ChemoBiolysis-0.0.11111111111/ChemoBiolysis.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      266 2024-03-14 19:48:07.000000 ChemoBiolysis-0.0.11111111111/ChemoBiolysis.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-14 19:48:07.000000 ChemoBiolysis-0.0.11111111111/ChemoBiolysis.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      240 2024-03-14 19:48:07.000000 ChemoBiolysis-0.0.11111111111/ChemoBiolysis.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2024-03-14 19:48:07.000000 ChemoBiolysis-0.0.11111111111/ChemoBiolysis.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1053 2023-12-09 17:25:26.000000 ChemoBiolysis-0.0.11111111111/LICENCE.txt
--rw-rw-rw-   0        0        0       26 2023-12-09 17:19:48.000000 ChemoBiolysis-0.0.11111111111/MANIFEST.in
--rw-rw-rw-   0        0        0     2768 2024-03-14 19:48:07.914680 ChemoBiolysis-0.0.11111111111/PKG-INFO
--rw-rw-rw-   0        0        0     2053 2023-12-15 19:14:47.000000 ChemoBiolysis-0.0.11111111111/README.md
--rw-rw-rw-   0        0        0       42 2024-03-14 19:48:07.916867 ChemoBiolysis-0.0.11111111111/setup.cfg
--rw-rw-rw-   0        0        0     1436 2024-03-14 19:47:09.000000 ChemoBiolysis-0.0.11111111111/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-01 13:32:53.433894 ChemoBiolysis-0.0.2/
+-rw-rw-rw-   0        0        0       84 2023-12-14 04:42:20.000000 ChemoBiolysis-0.0.2/CHANGELOG.txt
+drwxrwxrwx   0        0        0        0 2024-04-01 13:32:53.390847 ChemoBiolysis-0.0.2/ChemoBiolysis/
+-rw-rw-rw-   0        0        0    88834 2024-04-01 03:38:57.000000 ChemoBiolysis-0.0.2/ChemoBiolysis/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-01 13:32:53.429907 ChemoBiolysis-0.0.2/ChemoBiolysis.egg-info/
+-rw-rw-rw-   0        0        0     2758 2024-04-01 13:32:53.000000 ChemoBiolysis-0.0.2/ChemoBiolysis.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      266 2024-04-01 13:32:53.000000 ChemoBiolysis-0.0.2/ChemoBiolysis.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-01 13:32:53.000000 ChemoBiolysis-0.0.2/ChemoBiolysis.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      240 2024-04-01 13:32:53.000000 ChemoBiolysis-0.0.2/ChemoBiolysis.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2024-04-01 13:32:53.000000 ChemoBiolysis-0.0.2/ChemoBiolysis.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1053 2023-12-09 17:25:26.000000 ChemoBiolysis-0.0.2/LICENCE.txt
+-rw-rw-rw-   0        0        0       26 2023-12-09 17:19:48.000000 ChemoBiolysis-0.0.2/MANIFEST.in
+-rw-rw-rw-   0        0        0     2758 2024-04-01 13:32:53.431928 ChemoBiolysis-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0     2053 2023-12-15 19:14:47.000000 ChemoBiolysis-0.0.2/README.md
+-rw-rw-rw-   0        0        0       42 2024-04-01 13:32:53.433894 ChemoBiolysis-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0     1426 2024-04-01 13:31:58.000000 ChemoBiolysis-0.0.2/setup.py
```

### Comparing `ChemoBiolysis-0.0.11111111111/ChemoBiolysis/__init__.py` & `ChemoBiolysis-0.0.2/ChemoBiolysis/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -409,22 +409,29 @@
     substance_id = str(substance_id)
     inactive_url = f"https://pubchem.ncbi.nlm.nih.gov/rest/pug/assay/aid/{substance_id}/sids/txt?sids_type=inactive"
     response = requests.get(inactive_url)
     inactive_sids = response.text.split()
 
     print("Inactive sample SIDs:\n", inactive_sids)
     return inactive_url
-def qspr_analysis(csv_file_path, smiles_column_name, dependent_variable_column):
+import pandas as pd
+from rdkit import Chem
+from rdkit.Chem import Descriptors
+from rdkit.Chem import rdMolDescriptors
+import statsmodels.api as sm
+
+def qspr_analysis(csv_file_path, smiles_column_name, dependent_variable_column, additional_independent_variable=None):
     # Create descriptor instances
-    zagreb_index1 = ZagrebIndex.ZagrebIndex(version=1)
-    zagreb_index2 = ZagrebIndex.ZagrebIndex(version=2)
-    wiener_index = WienerIndex.WienerIndex()
+    zagreb_index1 = rdMolDescriptors.CalcNumAromaticRings
+    zagreb_index2 = rdMolDescriptors.CalcNumRotatableBonds
+    wiener_index = Descriptors.MolWt
 
     # Read the CSV file into a pandas dataframe
     df = pd.read_csv(csv_file_path)
+    display(df)
 
     # Create lists to store calculated results
     result_Wiener = []
     result_Z1 = []
     result_Z2 = []
 
     # Iterate through each row of the CSV data
@@ -444,42 +451,53 @@
 
     # Save the dataframe as a CSV file
     output_csv_path = f"{csv_file_path}_W_Z1_Z2_qspr_analysis_results.csv"
     df.to_csv(output_csv_path, index=False)
     display(df)
 
     # Perform QSPR analysis
-    independent_variables = ["MW", "Wiener", "Z1", "Z2"]
+    independent_variables = [ "Wiener", "Z1", "Z2"]
+    if additional_independent_variable:
+        independent_variables.append(additional_independent_variable)
     X = df[independent_variables]        # select our independent variables
     X = sm.add_constant(X)               # add an intercept to our model
     y = df[[dependent_variable_column]]  # select the dependent variable
     model = sm.OLS(y, X).fit()            # set up our model
 
     # Save the model summary to a text file
     output_text_path = f"{csv_file_path}_W_Z1_Z2_model_summary.txt"
     with open(output_text_path, "w") as text_file:
         text_file.write(model.summary().as_text())
         print(model.summary())
 
     print(f"\n***Results saved to:\n- CSV file: {output_csv_path}\n- Model summary text file: {output_text_path}")
 
-    result=(f"\n***Results saved to:\n- CSV file: {output_csv_path}\n- Model summary text file: {output_text_path}")
-    return str(result)
-#qspr_analysis('BPP.csv','SS', 'BP_K' )
+    result = f"\n***Results saved to:\n- CSV file: {output_csv_path}\n- Model summary text file: {output_text_path}"
+    return result
+
+# Example usage:
+# qspr_analysis("BPP.csv","SS","BP_K","MW")
+
+
+import pandas as pd
+from rdkit import Chem
+from rdkit.Chem import Descriptors
+from rdkit.Chem import rdMolDescriptors
+import statsmodels.api as sm
 
-def qspr_analysis_2(csv_file_path, dependent_variable_column,  smiles_column_name, descriptor_types):
+def qspr_analysis_2(csv_file_path, dependent_variable_column, smiles_column_name, descriptor_types, additional_independent_variables=None):
     # Create descriptor instances based on user's choice
     descriptor_instances = []
     for descriptor_type in descriptor_types:
         if descriptor_type == "z1":
-            descriptor_instances.append(ZagrebIndex.ZagrebIndex(version=1))
+            descriptor_instances.append(rdMolDescriptors.CalcNumAromaticRings)
         elif descriptor_type == "z2":
-            descriptor_instances.append(ZagrebIndex.ZagrebIndex(version=2))
+            descriptor_instances.append(rdMolDescriptors.CalcNumRotatableBonds)
         elif descriptor_type == "w":
-            descriptor_instances.append(WienerIndex.WienerIndex())
+            descriptor_instances.append(Descriptors.MolWt)
         else:
             raise ValueError(f"Invalid descriptor type '{descriptor_type}'. Choose 'z1', 'z2', or 'w'.")
 
     # Read the CSV file into a pandas dataframe
     df = pd.read_csv(csv_file_path)
 
     # Create lists to store calculated results
@@ -493,36 +511,50 @@
 
             # Calculate descriptor values
             result_descriptor.append(descriptor_instance(mol))
 
         # Add the calculated results to the dataframe
         df[descriptor_type.capitalize()] = result_descriptor
 
+    # Calculate additional independent variables if provided
+    if additional_independent_variables:
+        if "MW" in additional_independent_variables:
+            mw_values = []
+            for index, row in df.iterrows():
+                SMILE = row[smiles_column_name]
+                mol = Chem.MolFromSmiles(SMILE)
+                mw_values.append(Descriptors.MolWt(mol))
+            df["MW"] = mw_values
+
     # Save the dataframe as a CSV file
     output_csv_path = f"{csv_file_path}_qspr_analysis_results.csv"
     df.to_csv(output_csv_path, index=False)
     display(df)
 
     # Perform QSPR analysis
-    independent_variables = ["MW"] + [desc.capitalize() for desc in descriptor_types]
+    independent_variables = [desc.capitalize() for desc in descriptor_types]
+    if additional_independent_variables:
+        independent_variables += ["MW"]
     X = df[independent_variables]        # select our independent variables
     X = sm.add_constant(X)               # add an intercept to our model
     y = df[[dependent_variable_column]]  # select the dependent variable
     model = sm.OLS(y, X).fit()            # set up our model
 
     # Save the model summary to a text file
     output_text_path = f"{csv_file_path}_model_summary.txt"
     with open(output_text_path, "w") as text_file:
         text_file.write(model.summary().as_text())
         print(model.summary())
 
     print(f"\n***Results saved to:\n- CSV file: {output_csv_path}\n- Model summary text file: {output_text_path}")
     result = (f"\n***Results saved to:\n- CSV file: {output_csv_path}\n- Model summary text file: {output_text_path}")
     return str(result)
-#qspr_analysis_2('BPP.csv', 'BP_K', 'SS', ['z1', 'z2', 'w'] )
+
+# Example usage:
+#qspr_analysis_2('BPP.csv', 'BP_K', 'SS', ['z1', 'z2', 'w'], ["MW"])
 
 
 def predict_candidate_active_chemicals(assay_id):
     # Step 1: Retrieve CIDs from the first link
     cid_url = f"https://pubchem.ncbi.nlm.nih.gov/rest/pug/assay/aid/{assay_id}/cids/txt?cids_type=active"
     cid_response = requests.get(cid_url)
     cid_list = cid_response.text.split()
@@ -1080,16 +1112,15 @@
     X_filtered = selection.fit_transform(X)
     return X_filtered
 
 # Function for lazy imports of specific modules
 def lazy_imports():
     global train_test_split, LabelEncoder
 
-# Main function for analyzing bioassay using machine learning
-def analyze_bioassay_ml(aid, output_file=None):
+def pubchem_bioact_desc_ml_classify(aid, output_file=None):
     # Function to convert AID to CIDs for both active and inactive compounds
     def aid_to_cids(aid):
         url_active = f"https://pubchem.ncbi.nlm.nih.gov/rest/pug/assay/aid/{aid}/cids/txt?cids_type=active"
         url_inactive = f"https://pubchem.ncbi.nlm.nih.gov/rest/pug/assay/aid/{aid}/cids/txt?cids_type=inactive"
 
         response_active = requests.get(url_active)
         response_inactive = requests.get(url_inactive)
@@ -1236,16 +1267,17 @@
         sns.heatmap(cf_matrix, annot=True, cmap='Blues', xticklabels=list(target_meanings.values()), yticklabels=list(target_meanings.values()))
         plt.xlabel('Predicted')
         plt.ylabel('True')
         plt.title('Confusion Matrix')
         plt.show()
 
         print(classification_report(y_test, y_pred_class))
-        return#aid_number = 1000
-#analyze_bioassay_ml(aid_number, output_file='Machine_learning_for_bioassay_1000.csv')
+        return
+
+#pubchem_bioact_desc_ml_classify(1000)
 
 def perform_classification(csv_file_path):
     # Open and display the CSV file
     df = pd.read_csv(csv_file_path)
 
     # Encode the 'Status' column if needed
     if 'Status' in df.columns:
@@ -1415,14 +1447,15 @@
     plt.title('Confusion Matrix')
     plt.show()
 
     print(classification_report(y_test, y_pred_class))
     return
 
 
+
     #aid_input = input("Enter the AID: ")
 
 
 def perform_classification(csv_file_path):
     # Open and display the CSV file
     df = pd.read_csv(csv_file_path)
 
@@ -1617,8 +1650,677 @@
 
         filename = f"{file_path}_lig{idx}_{mycid}.mol"
         Chem.MolToMolFile(mymol, filename)
 
     df.to_csv('Virtual_Screening.csv', index=False)
     print("Now, you can find 'Virtual_Screening.csv' in your device")
 
-    return df.to_csv('Virtual_Screening.csv')
+    return df.to_csv('Virtual_Screening.csv')
+
+
+import pandas as pd
+from rdkit import Chem
+from rdkit.Chem import Draw
+from rdkit.Chem import rdFMCS
+
+def read_csv_and_find_common_substructure(csv_file_path):
+    """
+    Reads a CSV file containing SMILES representations of compounds and finds the common substructure.
+
+    Parameters:
+    - csv_file_path (str): Path to the CSV file containing SMILES representations.
+
+    Returns:
+    - None
+    """
+
+    # Read CSV file
+    df = pd.read_csv(csv_file_path)
+    display(df)
+
+    # Extract SMILES from the DataFrame
+    smiles_list = df['PUBCHEM_EXT_DATASOURCE_SMILES'].tolist()
+
+    # Convert SMILES to RDKit molecules
+    # Convert SMILES to RDKit molecules, skipping empty cells
+    # Convert valid SMILES to RDKit molecules
+    molecules = []
+    for smiles in smiles_list:
+        if isinstance(smiles, str) and smiles.strip():  # Check if it's a non-empty string
+            mol = Chem.MolFromSmiles(smiles)
+            if mol:
+                molecules.append(mol)
+
+    # Draw molecules
+    grid_image = Draw.MolsToGridImage(molecules, molsPerRow=5, subImgSize=(400, 400))
+    display(grid_image)
+
+    # Find common substructure
+    mcs_result = rdFMCS.FindMCS(molecules, threshold=0.7)
+    common_substructure = Chem.MolFromSmarts(mcs_result.smartsString)
+
+    print("The common substructure for these compounds:")
+    display(common_substructure)
+
+# Example usage:
+#read_csv_and_find_common_substructure("AID_1860_datatable_inactive.csv")
+import pandas as pd
+from rdkit import Chem
+
+def visualize_molecules_from_smiles(file_path, smiles_column):
+    """
+    Visualize molecules from SMILES strings in a CSV file.
+
+    Parameters:
+        file_path (str): Path to the CSV file containing molecular data.
+        smiles_column (str): Name of the column containing SMILES strings.
+
+    Returns:
+        None
+    """
+    # Read CSV file
+    df = pd.read_csv(file_path)
+
+    # Extract SMILES from the DataFrame
+    smiles_list = df[smiles_column].tolist()
+
+    # Convert SMILES to RDKit molecules, skipping empty cells
+    molecules = [Chem.MolFromSmiles(smiles) for smiles in smiles_list if isinstance(smiles, str) and smiles.strip()]
+
+    # Draw molecules
+    grid_image = Draw.MolsToGridImage(molecules, molsPerRow=5, subImgSize=(400, 400))
+    display(grid_image)
+
+# Example Usage:
+#file_path = "dataset_ise.csv"
+#visualize_molecules_from_smiles(file_path, "smiles")
+
+def virtual_screening_2(csv_file, smiles_column):
+    # Read CSV file
+    df = pd.read_csv(csv_file, header=None)
+    df_act = df.copy()
+
+    # Display DataFrame
+    print("DataFrame:")
+    display(df)
+
+    # Extract SMILES strings
+    smiles_act = df[smiles_column].tolist()
+
+    # Print number of structures in DataFrame
+    print("Number of structures in the DataFrame:", len(df))
+
+    prolog = "https://pubchem.ncbi.nlm.nih.gov/rest/pug"
+    cids_hit = dict()
+
+    for idx, mysmiles in enumerate(smiles_act):
+        mydata = {'smiles': mysmiles}
+        url = f"{prolog}/compound/fastsimilarity_2d/smiles/cids/txt"
+        print("Request URL:", url)  # Print request URL
+
+        res = requests.post(url, data=mydata)
+
+        # Handle response status code
+        if res.status_code == 200:
+            cids = res.text.split()
+            cids = [int(x) for x in cids]  # Convert CIDs from string to integer.
+        else:
+            # Print error information
+            print("Error at index", idx, "with SMILES:", mysmiles)
+            print("Status code:", res.status_code)
+            print("Content:", res.content)
+            continue
+
+        # Update cids_hit dictionary
+        for mycid in cids:
+            cids_hit[mycid] = cids_hit.get(mycid, 0) + 1
+
+        time.sleep(0.2)
+
+    # Sort the dictionary by frequency
+    sorted_by_freq = [(v, k) for k, v in cids_hit.items()]
+    sorted_by_freq.sort(reverse=True)
+
+    # Print the top 10 results
+    print("Top 10 results (frequency, CID):")
+    for v, k in enumerate(sorted_by_freq[:10]):
+        print(v, k)  # Print (frequency, CID)
+
+    cids_query = dict()
+
+    for idx, mysmiles in enumerate(smiles_act):
+
+        mydata = {'smiles': mysmiles}
+        url = prolog + "/compound/fastidentity/smiles/cids/txt?identity_type=same_connectivity"
+        res = requests.post(url, data=mydata)
+
+        if (res.status_code == 200):
+            cids = res.text.split()
+            cids = [int(x) for x in cids]
+        else:
+            print("Error at", idx, ":", df_act.loc[idx, smiles_column], mysmiles)  # Using smiles_column instead of k
+            print(res.status_code)
+            print(res.content)
+
+        for mycid in cids:
+            cids_query[mycid] = cids_query.get(mycid, 0) + 1
+
+        time.sleep(0.2)
+        sorted_by_freq = [(v, k) for k, v in cids_hit.items()]
+        sorted_by_freq.sort(reverse=True)
+
+        for v, k in enumerate(sorted_by_freq):
+
+            if v == 10:
+                break
+
+            print(v, k)  # Print (frequency, CID)
+    sorted_by_freq = [(v, k) for k, v in cids_hit.items()]
+    sorted_by_freq.sort(reverse=True)
+
+    for v, k in enumerate(sorted_by_freq):
+
+        if v == 10:
+            break
+
+        print(v, k)  # Print (frequency, CID)
+
+    cids_query = dict()
+
+    for idx, mysmiles in enumerate(smiles_act):
+
+        mydata = {'smiles': mysmiles}
+        url = prolog + "/compound/fastidentity/smiles/cids/txt?identity_type=same_connectivity"
+        res = requests.post(url, data=mydata)
+
+        if (res.status_code == 200):
+            cids = res.text.split()
+            cids = [int(x) for x in cids]
+        else:
+            print("Error at", idx, ":", df_act.loc[idx, smiles_column], mysmiles)  # Using smiles_column instead of k
+            print(res.status_code)
+            print(res.content)
+
+        for mycid in cids:
+            cids_query[mycid] = cids_query.get(mycid, 0) + 1
+
+        time.sleep(0.2)
+
+    len(cids_query.keys())  # Show the number of CIDs that represent the query compounds.
+    for mycid in cids_query.keys():
+        cids_hit.pop(mycid, None)
+    len(cids_hit)
+
+    sorted_by_freq = [(v, k) for k, v in cids_hit.items()]
+    sorted_by_freq.sort(reverse=True)
+
+    for v, k in enumerate(sorted_by_freq):
+
+        if v == 10:
+            break
+
+        print(v, k)  # Print (frequency, CID)
+    sorted_by_freq = [(v, k) for k, v in cids_hit.items()]
+    sorted_by_freq.sort(reverse=True)
+
+    for v, k in enumerate(sorted_by_freq):
+
+        if v == 10:
+            break
+
+        print(v, k)  # Print (frequency, CID)
+
+    chunk_size = 100
+
+    if (len(cids_hit) % chunk_size == 0):
+        num_chunks = len(cids_hit) // chunk_size
+    else:
+        num_chunks = len(cids_hit) // chunk_size + 1
+
+    cids_list = list(cids_hit.keys())
+
+    print("# Number of chunks:", num_chunks)
+
+    csv = ""  # sets a variable called csv to save the comma separated output
+
+    for i in range(num_chunks):
+
+        print(i, end=" ")
+
+        idx1 = chunk_size * i
+        idx2 = chunk_size * (i + 1)
+
+        cids_str = ",".join([str(x) for x in cids_list[idx1:idx2]])  # build pug input for chunks of data
+        url = prolog + "/compound/cid/" + cids_str + "/property/HBondDonorCount,HBondAcceptorCount,MolecularWeight,XLogP,CanonicalSMILES,IsomericSMILES/csv"
+
+        res = requests.get(url)
+
+        if (i == 0):  # if this is the first request, store result in empty csv variable
+            csv = res.text
+        else:  # if this is a subsequent request, add the request to the csv variable adding a new line between chunks
+            csv = csv + "\n".join(res.text.split()[1:]) + "\n"
+
+        time.sleep(0.2)
+
+    # print(csv)
+    from io import StringIO
+
+    csv_file = StringIO(csv)
+
+    df_raw = pd.read_csv(csv_file, sep=",")
+
+    df_raw.shape  # Show the shape (dimesnion) of the data frame
+    df_raw.isna().sum()  # Check if there are any NULL values.
+    len(df_raw)  # Check the number of rows (which is equals to the number of CIDs)
+    # First load the cids_hit dictionary into a data frame.
+    df_freq = pd.DataFrame(cids_hit.items(), columns=['CID', 'HitFreq'])
+    df_freq.head(5)
+    # Double-check if the data are loaded correctly
+    # Compare the data with those from Cell [12]
+    df_freq.sort_values(by=['HitFreq', 'CID'], ascending=False).head(10)
+    # Create a new data frame called "df" by joining the df and df_freq data frames
+    df = df_raw.join(df_freq.set_index('CID'), on='CID')
+    df.shape
+    df.sort_values(by=['HitFreq', 'CID'], ascending=False).head(10)
+    df = df[(df['HBondDonorCount'] <= 5) &
+            (df['HBondAcceptorCount'] <= 10) &
+            (df['MolecularWeight'] <= 500) &
+            (df['XLogP'] < 5)]
+    # Draw the structures of the top 10 compounds
+
+    cids_top = df.sort_values(by=['HitFreq', 'CID'], ascending=False).head(10).CID.to_list()
+    mols = []
+
+    for mycid in cids_top:
+        mysmiles = df[df.CID == mycid].IsomericSMILES.item()
+
+        mol = Chem.MolFromSmiles(mysmiles)
+        Chem.FindPotentialStereoBonds(mol)  # Identify potential stereo bonds!
+        mols.append(mol)
+
+    mylegends = ["CID " + str(x) for x in cids_top]
+    img = Draw.MolsToGridImage(mols, molsPerRow=2, subImgSize=(400, 400), legends=mylegends)
+    display(img)
+
+    # Extract unique compounds in terms of canonical SMILES
+
+    canonical_smiles = df.CanonicalSMILES.unique()
+    idx_to_include = []
+
+    for mysmiles in canonical_smiles:
+        myidx = df[df.CanonicalSMILES == mysmiles].index.to_list()[0]
+
+        idx_to_include.append(myidx)
+    # Create a new column 'Include'
+    # All values initialized to 0 (not include)
+    df['Include'] = 0
+    df['Include'].sum()
+    # Now the "Include" column's value is modified if the record is in the idx_to_include list.
+    df.loc[idx_to_include, 'Include'] = 1
+    df['Include'].sum()
+    # Now draw the top 10 unique compounds (in terms of canonical SMILES)
+    cids_top = df[df['Include'] == 1].sort_values(by=['HitFreq', 'CID'], ascending=False).head(10).CID.to_list()
+    mols = []
+
+    for mycid in cids_top:
+        mysmiles = df[df.CID == mycid].IsomericSMILES.item()
+
+        mol = Chem.MolFromSmiles(mysmiles)
+        Chem.FindPotentialStereoBonds(mol)  # Identify potential stereo bonds!
+        mols.append(mol)
+
+    mylegends = ["CID " + str(x) for x in cids_top]
+    img = Draw.MolsToGridImage(mols, molsPerRow=2, subImgSize=(400, 400), legends=mylegends)
+    display(img)
+
+    from rdkit.Chem import AllChem
+
+    for idx, mycid in enumerate(cids_top):
+
+        if idx == 3:
+            break
+
+        mysmiles = df[df['CID'] == mycid].IsomericSMILES.item()
+
+        mymol = Chem.MolFromSmiles(mysmiles)
+        mymol = Chem.AddHs(mymol)
+        AllChem.EmbedMolecule(mymol)
+        AllChem.MMFFOptimizeMolecule(mymol)
+
+        filename = "screenig result" + str(idx) + "_" + str(mycid) + ".mol"
+        Chem.MolToMolFile(mymol, filename)
+    df.to_csv('screening result.csv')
+
+
+# Example usage:
+#csv_file = "AID_1107225_datatable_active.csv"  # Path to your CSV file
+#smiles_column = 3  # Index of the column containing SMILES strings (assuming it's the fourth column)
+#virtual_screening_2(csv_file, smiles_column)
+from rdkit.Chem import AllChem  # Add this import statement
+
+def virtual_screening_3(csv_file, smiles_column):
+    # Read CSV file
+    df = pd.read_csv(csv_file)
+    df_act = df.copy()
+
+    # Display DataFrame
+    print("DataFrame:")
+    display(df)
+
+    # Extract SMILES strings
+    smiles_act = df[smiles_column].tolist()
+
+    # Print number of structures in DataFrame
+    print("Number of structures in the DataFrame:", len(df))
+
+    prolog = "https://pubchem.ncbi.nlm.nih.gov/rest/pug"
+    cids_hit = dict()
+
+    # Perform similarity search
+    for idx, mysmiles in enumerate(smiles_act):
+        mydata = {'smiles': mysmiles}
+        url = f"{prolog}/compound/fastsimilarity_2d/smiles/cids/txt"
+        print("Request URL:", url)  # Print request URL
+
+        res = requests.post(url, data=mydata)
+
+        # Handle response status code
+        if res.status_code == 200:
+            cids = res.text.split()
+            cids = [int(x) for x in cids]  # Convert CIDs from string to integer.
+        else:
+            # Print error information
+            print("Error at index", idx, "with SMILES:", mysmiles)
+            print("Status code:", res.status_code)
+            print("Content:", res.content)
+            continue
+
+        # Update cids_hit dictionary
+        for mycid in cids:
+            cids_hit[mycid] = cids_hit.get(mycid, 0) + 1
+
+        time.sleep(0.2)
+
+    # Sort the dictionary by frequency
+    sorted_by_freq = [(v, k) for k, v in cids_hit.items()]
+    sorted_by_freq.sort(reverse=True)
+
+    # Print the top 10 results of similarity search
+    print("Top 10 results of similarity search (frequency, CID):")
+    for v, k in enumerate(sorted_by_freq[:10]):
+        print(v, k)  # Print (frequency, CID)
+
+    cids_query = dict()
+
+    # Perform query using fast identity search
+    for idx, mysmiles in enumerate(smiles_act):
+        mydata = {'smiles': mysmiles}
+        url = prolog + "/compound/fastidentity/smiles/cids/txt?identity_type=same_connectivity"
+        res = requests.post(url, data=mydata)
+
+        if res.status_code == 200:
+            cids = res.text.split()
+            cids = [int(x) for x in cids]
+        else:
+            print("Error at", idx, ":", df_act.loc[idx, smiles_column], mysmiles)
+            print(res.status_code)
+            print(res.content)
+
+        for mycid in cids:
+            cids_query[mycid] = cids_query.get(mycid, 0) + 1
+
+        time.sleep(0.2)
+
+    # Sort and print the top 10 results of the query
+    sorted_by_freq = [(v, k) for k, v in cids_hit.items()]
+    sorted_by_freq.sort(reverse=True)
+    print("Top 10 results of query (frequency, CID):")
+    for v, k in enumerate(sorted_by_freq[:10]):
+        print(v, k)  # Print (frequency, CID)
+# Process remaining operations...
+
+    # Calculate the number of chunks for API requests
+    chunk_size = 100
+    if len(cids_hit) % chunk_size == 0:
+        num_chunks = len(cids_hit) // chunk_size
+    else:
+        num_chunks = len(cids_hit) // chunk_size + 1
+
+    cids_list = list(cids_hit.keys())
+
+    print("# Number of chunks:", num_chunks )
+
+    csv = ""   # Initialize a variable to save the comma-separated output
+
+    # Perform API requests in chunks
+    for i in range(num_chunks):
+
+        print(i, end=" ")
+
+        idx1 = chunk_size * i
+        idx2 = chunk_size * (i + 1)
+
+        cids_str = ",".join([str(x) for x in cids_list[idx1:idx2]])  # Build PUG input for chunks of data
+        url = prolog + f"/compound/cid/{cids_str}/property/HBondDonorCount,HBondAcceptorCount,MolecularWeight,XLogP,CanonicalSMILES,IsomericSMILES/csv"
+
+        res = requests.get(url)
+
+        if i == 0:  # If this is the first request, store result in empty csv variable
+            csv = res.text
+        else:       # If this is a subsequent request, add the request to the csv variable adding a new line between chunks
+            csv = csv + "\n".join(res.text.split()[1:]) + "\n"
+
+        time.sleep(0.2)
+
+    # Read CSV file from string
+    from io import StringIO
+    csv_file = StringIO(csv)
+    df_raw = pd.read_csv(csv_file, sep=",")
+
+    # Further operations on df_raw
+    df_raw_shape = df_raw.shape    # Show the shape (dimension) of the data frame
+    df_raw_na_sum = df_raw.isna().sum()    # Check if there are any NULL values.
+    df_raw_len = len(df_raw)    # Check the number of rows (which is equals to the number of CIDs)
+
+    # Load the cids_hit dictionary into a data frame
+    df_freq = pd.DataFrame(cids_hit.items(), columns=['CID','HitFreq'])
+    df_freq_head = df_freq.head(5)  # Display first 5 rows
+    df_freq_sorted = df_freq.sort_values(by=['HitFreq', 'CID'], ascending=False).head(10)  # Sort and display top 10 rows
+
+    # Create a new data frame called "df" by joining the df_raw and df_freq data frames
+    df = df_raw.join(df_freq.set_index('CID'), on='CID')
+    df_shape = df.shape
+    df_top_sorted = df.sort_values(by=['HitFreq', 'CID'], ascending=False).head(10)
+
+    # Filter df based on conditions
+    df_filtered = df[(df['HBondDonorCount'] <= 5) &
+                     (df['HBondAcceptorCount'] <= 10) &
+                     (df['MolecularWeight'] <= 500) &
+                     (df['XLogP'] < 5)]
+
+    # Draw the structures of the top 10 compounds
+    cids_top = df_filtered.sort_values(by=['HitFreq', 'CID'], ascending=False).head(10).CID.to_list()
+    mols = []
+
+    for mycid in cids_top:
+        mysmiles = df[df.CID == mycid].IsomericSMILES.item()
+        mol = Chem.MolFromSmiles(mysmiles)
+        Chem.FindPotentialStereoBonds(mol)    # Identify potential stereo bonds!
+        mols.append(mol)
+
+    mylegends = ["CID " + str(x) for x in cids_top]
+    img = Draw.MolsToGridImage(mols, molsPerRow=2, subImgSize=(400,400), legends=mylegends)
+    display(img)
+
+    # Extract unique compounds in terms of canonical SMILES
+    canonical_smiles = df_filtered.CanonicalSMILES.unique()
+    idx_to_include = []
+
+    for mysmiles in canonical_smiles:
+        myidx = df_filtered[df_filtered.CanonicalSMILES == mysmiles].index.to_list()[0]
+        idx_to_include.append(myidx)
+
+    # Create a new column 'Include'
+    # All values initialized to 0 (not include)
+    df_filtered['Include'] = 0
+    df_filtered.loc[idx_to_include, 'Include'] = 1  # Set 'Include' column's value to 1 if the record is in the idx_to_include list
+
+    # Draw the top 10 unique compounds (in terms of canonical SMILES)
+    cids_top_unique = df_filtered[df_filtered['Include'] == 1].sort_values(by=['HitFreq', 'CID'], ascending=False).head(10).CID.to_list()
+    mols = []
+
+    for mycid in cids_top_unique:
+        mysmiles = df_filtered[df_filtered.CID == mycid].IsomericSMILES.item()
+        mol = Chem.MolFromSmiles(mysmiles)
+        Chem.FindPotentialStereoBonds(mol)    # Identify potential stereo bonds!
+        mols.append(mol)
+
+    mylegends = ["CID " + str(x) for x in cids_top_unique]
+    img = Draw.MolsToGridImage(mols, molsPerRow=2, subImgSize=(400,400), legends=mylegends)
+    display(img)
+
+    # Generate and save 3D structures of the top 3 compounds
+    for idx, mycid in enumerate(cids_top_unique):
+        if idx == 3 :
+            break
+
+        mysmiles = df[ df['CID'] == mycid ].IsomericSMILES.item()
+
+        mymol = Chem.MolFromSmiles(mysmiles)
+        mymol = Chem.AddHs(mymol)
+        AllChem.EmbedMolecule(mymol)
+        AllChem.MMFFOptimizeMolecule(mymol)
+
+        filename = "screenig result" + str(idx) + "_" + str(mycid) + ".mol"
+        Chem.MolToMolFile(mymol, filename)
+    df.to_csv('screening result.csv')
+
+
+    # Save the final filtered dataframe to CSV
+    df_filtered.to_csv('screening_result.csv')
+
+# Example usage:
+#csv_file = "AID_1107225_datatable_active.csv"  # Path to your CSV file
+#smiles_column = "PUBCHEM_EXT_DATASOURCE_SMILES"  # Index of the column containing SMILES strings
+#virtual_screening_3(csv_file, smiles_column)
+import pandas as pd
+from rdkit import Chem
+from rdkit.Chem import Descriptors
+
+
+def process_csv_and_compute_RDKit_descriptors(input_csv, smiles_column):
+    # Read CSV file
+    df = pd.read_csv(input_csv)
+
+    # Remove rows with empty cells in the SMILES column
+    df = df.dropna(subset=[smiles_column])
+
+    # Extract SMILES strings
+    smiles_list = df[smiles_column].tolist()
+
+    # Convert SMILES strings into RDKit molecules
+    molecules = [Chem.MolFromSmiles(smi) for smi in smiles_list]
+
+    # Calculate RDKit descriptors
+    descriptor_names = [desc[0] for desc in Descriptors.descList]
+    descriptor_values = [[desc[1](mol) for desc in Descriptors.descList] for mol in molecules]
+
+    # Create DataFrame with descriptors
+    descriptor_df = pd.DataFrame(descriptor_values, columns=descriptor_names)
+
+    # Combine descriptors with original data
+    df_with_descriptors = pd.concat([df.reset_index(drop=True), descriptor_df], axis=1)
+
+    # Save the processed data to a new CSV file
+    output_csv = input_csv.replace('.csv', '_processed.csv')
+    df_with_descriptors.to_csv(output_csv, index=False)
+
+
+# Example usage:
+#input_csv = "AID_1860_datatable_inactive.csv"
+#smiles_column = "SMILES"
+#process_csv_and_compute_descriptors(input_csv, smiles_column)
+import pandas as pd
+import mordred
+from rdkit import Chem
+from mordred import Calculator, descriptors
+
+
+def process_csv_and_compute_mordred_descriptors(input_csv, smiles_column):
+    # Read CSV file
+    df = pd.read_csv(input_csv)
+
+    # Remove rows with empty cells in the SMILES column
+    df = df.dropna(subset=[smiles_column])
+
+    # Extract SMILES strings
+    smiles_list = df[smiles_column].tolist()
+
+    # Convert SMILES strings into RDKit molecules
+    molecules = [Chem.MolFromSmiles(smi) for smi in smiles_list]
+
+    # Create a Mordred calculator object
+    calc = mordred.Calculator(mordred.descriptors, ignore_3D=False)
+
+    # Compute descriptors for each molecule
+    descriptor_values = calc.pandas(molecules)
+
+    # Combine descriptors with original data
+    df_with_descriptors = pd.concat([df.reset_index(drop=True), descriptor_values], axis=1)
+
+    # Save the processed data to a new CSV file
+    output_csv = input_csv.replace('.csv', '_processed.csv')
+    df_with_descriptors.to_csv(output_csv, index=False)
+
+    print(f"Processed data saved to {output_csv}")
+
+
+# Example usage:
+#input_csv = "AID_1860_datatable_inactive.csv"
+#smiles_column = "SMILES"
+#process_csv_and_compute_mordred_descriptors(input_csv, smiles_column)
+#df = pd.read_csv("AID_1860_datatable_inactive_processed.csv")
+#df
+
+
+import pandas as pd
+from rdkit import Chem
+from rdkit import DataStructs
+from rdkit.Chem import AllChem
+import numpy as np
+
+
+def process_csv_and_compute_morgan_fp(input_csv, smiles_column):
+    # Read CSV file
+    df = pd.read_csv(input_csv)
+
+    # Remove rows with empty cells in the SMILES column
+    df = df.dropna(subset=[smiles_column])
+
+    # Extract SMILES strings
+    smiles_list = df[smiles_column].tolist()
+
+    # Convert SMILES strings into RDKit molecules and compute Morgan fingerprints
+    Morgan_fpts = []
+    for smi in smiles_list:
+        mol = Chem.MolFromSmiles(smi)
+        fpts = AllChem.GetMorganFingerprintAsBitVect(mol, 2, 2048)
+        mfpts = np.array(fpts)
+        Morgan_fpts.append(mfpts)
+
+    # Create a DataFrame with Morgan fingerprints
+    Morgan_fp_df = pd.DataFrame(Morgan_fpts)
+
+    # Combine Morgan fingerprints with original data
+    df_with_fp = pd.concat([df.reset_index(drop=True), Morgan_fp_df], axis=1)
+
+    # Save the processed data to a new CSV file
+    output_csv = input_csv.replace('.csv', '_with_morgan_fp.csv')
+    df_with_fp.to_csv(output_csv, index=False)
+
+    print(f"Processed data with Morgan fingerprints saved to {output_csv}")
+
+
+# Example usage:
+#input_csv = "AID_1860_datatable_inactive.csv"
+#smiles_column = "SMILES"
+#process_csv_and_compute_morgan_fp(input_csv, smiles_column)
```

### Comparing `ChemoBiolysis-0.0.11111111111/ChemoBiolysis.egg-info/PKG-INFO` & `ChemoBiolysis-0.0.2/ChemoBiolysis.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ChemoBiolysis
-Version: 0.0.11111111111
+Version: 0.0.2
 Summary: ChemoBiolysis: A Comprehensive Python Package for Chemical and Biological Analysis
 Home-page: https://github.com/ahmed1212212/ChemoBiolysis.git
 Author: Ahmed Alhilal
 Author-email: aalhilal@udel.edu
 License: MIT
 Keywords: Cheminformatics
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `ChemoBiolysis-0.0.11111111111/LICENCE.txt` & `ChemoBiolysis-0.0.2/LICENCE.txt`

 * *Files identical despite different names*

### Comparing `ChemoBiolysis-0.0.11111111111/PKG-INFO` & `ChemoBiolysis-0.0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ChemoBiolysis
-Version: 0.0.11111111111
+Version: 0.0.2
 Summary: ChemoBiolysis: A Comprehensive Python Package for Chemical and Biological Analysis
 Home-page: https://github.com/ahmed1212212/ChemoBiolysis.git
 Author: Ahmed Alhilal
 Author-email: aalhilal@udel.edu
 License: MIT
 Keywords: Cheminformatics
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `ChemoBiolysis-0.0.11111111111/README.md` & `ChemoBiolysis-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `ChemoBiolysis-0.0.11111111111/setup.py` & `ChemoBiolysis-0.0.2/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,15 +6,15 @@
     'Operating System :: Microsoft :: Windows :: Windows 10',
     'License :: OSI Approved :: MIT License',
     'Programming Language :: Python :: 3'
 ]
 
 setup(
     name='ChemoBiolysis',
-    version='0.0.11111111111',
+    version='0.0.2',
     description='ChemoBiolysis: A Comprehensive Python Package for Chemical and Biological Analysis',
     long_description=open('README.md').read() + '\n\n' + open('CHANGELOG.txt').read(),
     url='https://github.com/ahmed1212212/ChemoBiolysis.git',
     author='Ahmed Alhilal',
     author_email='aalhilal@udel.edu',
     license='MIT',
     classifiers=classifiers,
```

