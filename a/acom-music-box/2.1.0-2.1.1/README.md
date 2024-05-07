# Comparing `tmp/acom_music_box-2.1.0.tar.gz` & `tmp/acom_music_box-2.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "acom_music_box-2.1.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "acom_music_box-2.1.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `acom_music_box-2.1.0.tar` & `acom_music_box-2.1.1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0    11357 2023-03-14 22:08:46.581988 acom_music_box-2.1.0/LICENSE
--rw-r--r--   0        0        0      792 2024-04-09 15:52:10.065732 acom_music_box-2.1.0/README.md
--rw-r--r--   0        0        0      414 2024-04-09 15:52:10.066098 acom_music_box-2.1.0/pyproject.toml
--rw-r--r--   0        0        0      858 2024-04-18 13:38:21.379266 acom_music_box-2.1.0/src/acom_music_box/__init__.py
--rw-r--r--   0        0        0    25087 2024-04-18 13:38:09.354114 acom_music_box-2.1.0/src/acom_music_box/music_box.py
--rw-r--r--   0        0        0     9227 2024-04-18 13:38:09.354683 acom_music_box-2.1.0/src/acom_music_box/music_box_conditions.py
--rw-r--r--   0        0        0     8301 2024-04-18 13:38:09.355332 acom_music_box-2.1.0/src/acom_music_box/music_box_evolving_conditions.py
--rw-r--r--   0        0        0     2511 2024-04-09 15:52:10.067450 acom_music_box-2.1.0/src/acom_music_box/music_box_model_options.py
--rw-r--r--   0        0        0      699 2024-04-09 15:52:10.067583 acom_music_box-2.1.0/src/acom_music_box/music_box_product.py
--rw-r--r--   0        0        0      615 2024-04-09 15:52:10.067829 acom_music_box-2.1.0/src/acom_music_box/music_box_reactant.py
--rw-r--r--   0        0        0     3284 2024-04-18 13:38:09.356246 acom_music_box-2.1.0/src/acom_music_box/music_box_reaction.py
--rw-r--r--   0        0        0     6542 2024-04-18 13:38:09.356739 acom_music_box-2.1.0/src/acom_music_box/music_box_reaction_list.py
--rw-r--r--   0        0        0      604 2024-04-09 15:52:10.068265 acom_music_box-2.1.0/src/acom_music_box/music_box_reaction_rate.py
--rw-r--r--   0        0        0     1211 2024-04-09 15:52:10.068390 acom_music_box-2.1.0/src/acom_music_box/music_box_species.py
--rw-r--r--   0        0        0      638 2024-04-09 15:52:10.068585 acom_music_box-2.1.0/src/acom_music_box/music_box_species_concentration.py
--rw-r--r--   0        0        0     3845 2024-04-12 20:15:10.522570 acom_music_box-2.1.0/src/acom_music_box/music_box_species_list.py
--rw-r--r--   0        0        0     3381 2024-04-09 15:52:10.068879 acom_music_box-2.1.0/src/acom_music_box/utils.py
--rw-r--r--   0        0        0     1098 1970-01-01 00:00:00.000000 acom_music_box-2.1.0/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-03-14 22:08:46.581988 acom_music_box-2.1.1/LICENSE
+-rw-r--r--   0        0        0     1788 2024-05-07 19:53:49.479730 acom_music_box-2.1.1/README.md
+-rw-r--r--   0        0        0      446 2024-05-07 20:02:12.547859 acom_music_box-2.1.1/pyproject.toml
+-rw-r--r--   0        0        0      858 2024-05-07 20:02:31.398430 acom_music_box-2.1.1/src/acom_music_box/__init__.py
+-rw-r--r--   0        0        0    27424 2024-04-30 15:52:16.190738 acom_music_box-2.1.1/src/acom_music_box/music_box.py
+-rw-r--r--   0        0        0    11008 2024-04-30 15:52:16.191512 acom_music_box-2.1.1/src/acom_music_box/music_box_conditions.py
+-rw-r--r--   0        0        0     9710 2024-04-30 15:52:16.192288 acom_music_box-2.1.1/src/acom_music_box/music_box_evolving_conditions.py
+-rw-r--r--   0        0        0     2881 2024-04-30 15:52:16.193336 acom_music_box-2.1.1/src/acom_music_box/music_box_model_options.py
+-rw-r--r--   0        0        0      699 2024-04-09 15:52:10.067583 acom_music_box-2.1.1/src/acom_music_box/music_box_product.py
+-rw-r--r--   0        0        0      615 2024-04-09 15:52:10.067829 acom_music_box-2.1.1/src/acom_music_box/music_box_reactant.py
+-rw-r--r--   0        0        0     8422 2024-04-30 15:52:16.193935 acom_music_box-2.1.1/src/acom_music_box/music_box_reaction.py
+-rw-r--r--   0        0        0     8909 2024-04-30 15:52:16.195245 acom_music_box-2.1.1/src/acom_music_box/music_box_reaction_list.py
+-rw-r--r--   0        0        0      604 2024-04-09 15:52:10.068265 acom_music_box-2.1.1/src/acom_music_box/music_box_reaction_rate.py
+-rw-r--r--   0        0        0     1211 2024-04-09 15:52:10.068390 acom_music_box-2.1.1/src/acom_music_box/music_box_species.py
+-rw-r--r--   0        0        0      638 2024-04-09 15:52:10.068585 acom_music_box-2.1.1/src/acom_music_box/music_box_species_concentration.py
+-rw-r--r--   0        0        0     4164 2024-04-30 15:52:16.196153 acom_music_box-2.1.1/src/acom_music_box/music_box_species_list.py
+-rw-r--r--   0        0        0     3381 2024-04-09 15:52:10.068879 acom_music_box-2.1.1/src/acom_music_box/utils.py
+-rw-r--r--   0        0        0     2128 1970-01-01 00:00:00.000000 acom_music_box-2.1.1/PKG-INFO
```

### Comparing `acom_music_box-2.1.0/LICENSE` & `acom_music_box-2.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `acom_music_box-2.1.0/src/acom_music_box/__init__.py` & `acom_music_box-2.1.1/src/acom_music_box/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """
 This is the music_box package.
 
 This package contains modules for handling various aspects of a music box, 
 including species, products, reactants, reactions, and more.
 """
-__version__ = "2.1.0"
+__version__ = "2.1.1"
 
 from .utils import convert_time, convert_pressure, convert_temperature, convert_concentration
 from .music_box_species import Species
 from .music_box_product import Product
 from .music_box_reactant import Reactant
 from .music_box_reaction import Reaction, Branched, Arrhenius, Tunneling, Troe_Ternary
 from .music_box_species_list import SpeciesList
```

### Comparing `acom_music_box-2.1.0/src/acom_music_box/music_box.py` & `acom_music_box-2.1.1/src/acom_music_box/music_box.py`

 * *Files 10% similar despite different names*

```diff
@@ -54,18 +54,21 @@
             conditions (Conditions): The associated conditions at the given time point.
         """
         evolving_condition = EvolvingConditions(time=[time_point], conditions=[conditions])
         self.evolvingConditions.append(evolving_condition)
 
     def generateConfig(self, directory):
         """
-        Generate configuration JSON for the box model simulation.
+        Generate configuration JSON for the box model simulation and writes it to files in the specified directory.
+
+        Args:
+            directory (str): The directory where the configuration files will be written.
 
         Returns:
-        tuple: A tuple containing the species configuration JSON and the reaction configuration JSON.
+            None
         """
         output_path = "./src/configs/" + directory
 
         # Check if directory exists and create it if it doesn't
         if not os.path.exists(output_path):
             os.makedirs(output_path)
             os.makedirs(output_path + "/camp_data")    
@@ -407,18 +410,28 @@
         """
         # Create a solver object using the configuration file
         self.solver = musica.create_micm(path_to_config)
 
 
     def solve(self, path_to_output = None):
         """
-        TODO: Solve the box model simulation.
+        Solves the box model simulation and optionally writes the output to a file.
+
+        This function runs the box model simulation using the current settings and 
+        conditions. If a path is provided, it writes the output of the simulation to 
+        the specified file.
+
+        Args:
+            path_to_output (str, optional): The path to the file where the output will 
+            be written. If None, no output file is created. Defaults to None.
+
+        Returns:
+            list: A 2D list where each inner list represents the results of the simulation 
+            at a specific time step.
         """
-        # TODO: Implement the logic to solve the box model simulation.
-        # Update the internal state of the BoxModel instance to reflect the simulation results.
 
         #sets up initial conditions to be current conditions
         curr_conditions = self.initial_conditions
 
         #sets up initial concentraion values
         curr_concentrations = self.initial_conditions.get_concentration_array()
 
@@ -519,17 +532,29 @@
                 writer.writerows(output_array)
         
         #returns output_array 
         return output_array
         
     def readFromUIJson(self, path_to_json):
         """
-        TODO: Read the box model configuration from json and sets config
+        Reads and parses a JSON file from the MusicBox Interactive UI to set up the box model simulation.
+
+        This function takes the path to a JSON file, reads the file, and parses the JSON 
+        to set up the box model simulation.
+
+        Args:
+            path_to_json (str): The path to the JSON file from the UI.
+
+        Returns:
+            None
+
+        Raises:
+            ValueError: If the JSON file cannot be read or parsed.
         """
-        # TODO: Implement the logic to update the box model config using a json.
+
 
         with open(path_to_json, 'r') as json_file:
             data = json.load(json_file)
 
             # Set box model options
             self.box_model_options = BoxModelOptions.from_UI_JSON(data)
 
@@ -543,17 +568,26 @@
             self.initial_conditions = Conditions.from_UI_JSON(data, self.species_list, self.reaction_list)
 
             # Set evolving conditions
             self.evolving_conditions = EvolvingConditions.from_UI_JSON(data, self.species_list, self.reaction_list)  
 
     def readFromUIJsonString(self, data):
         """
-        TODO: Read the box model configuration from json and sets config
+        Reads and parses a JSON string from the MusicBox Interactive UI to set up the box model simulation.
+
+        Args:
+            json_string (str): The JSON string from the UI.
+
+        Returns:
+            None
+
+        Raises:
+            ValueError: If the JSON string cannot be parsed.
         """
-        # TODO: Implement the logic to update the box model config using a json.
+  
 
         # Set box model options
         self.box_model_options = BoxModelOptions.from_UI_JSON(data)
 
         # Set species list
         self.species_list = SpeciesList.from_UI_JSON(data)
 
@@ -563,14 +597,26 @@
         # Set initial conditions
         self.initial_conditions = Conditions.from_UI_JSON(data, self.species_list, self.reaction_list)
 
         # Set evolving conditions
         self.evolving_conditions = EvolvingConditions.from_UI_JSON(data, self.species_list, self.reaction_list)    
 
     def readConditionsFromJson(self, path_to_json):
+        """
+        Reads and parses a JSON file from the CAMP JSON file to set up the box model simulation.
+
+        Args:
+            path_to_json (str): The JSON path to the JSON file.
+
+        Returns:
+            None
+
+        Raises:
+            ValueError: If the JSON string cannot be parsed.
+        """
 
         with open(path_to_json, 'r') as json_file:
             data = json.load(json_file)
             # Set box model options
             self.box_model_options = BoxModelOptions.from_config_JSON(data)
 
             # Set species list
@@ -582,21 +628,50 @@
             self.initial_conditions = Conditions.from_config_JSON(path_to_json, data, self.species_list, self.reaction_list)
 
             # Set initial conditions
             self.evolving_conditions = EvolvingConditions.from_config_JSON(path_to_json, data, self.species_list, self.reaction_list)
             
 
     def speciesOrdering(self):
+        """
+        Retrieves the ordering of species used in the solver.
+
+        This function calls the `species_ordering` function from the `musica` module, 
+        passing the solver instance from the current object.
+
+        Returns:
+            dict: The ordered dictionary of species used in the solver.
+        """
         return musica.species_ordering(self.solver)
 
     def userDefinedReactionRates(self):
-        return musica.user_defined_reaction_rates(self.solver)
-    
+        """
+        Retrieves the user-defined reaction rates from the solver.
+
+        This function calls the `user_defined_reaction_rates` function from the `musica` module, 
+        passing the solver instance from the current object.
+
+        Returns:
+            dict: The dictionary of user-defined reaction rates used in the solver.
+        """
     @classmethod
     def order_reaction_rates(self, curr_conditions, rate_constant_ordering):
+        """
+        Orders the reaction rates based on the provided ordering.
+
+        This function takes the current conditions and a specified ordering for the rate constants, 
+        and reorders the reaction rates accordingly.
+
+        Args:
+            rate_constants (dict): A dictionary of rate constants.
+            rate_constant_ordering (dict): A dictionary that maps rate constant keys to indices for ordering.
+
+        Returns:
+            list: An ordered list of rate constants.
+        """
         rate_constants = {}
         for rate in curr_conditions.reaction_rates:
 
             if(rate.reaction.reaction_type == "PHOTOLYSIS"):
                 key = "PHOTO." + rate.reaction.name
             elif(rate.reaction.reaction_type == "LOSS"):
                 key = "LOSS." + rate.reaction.name
```

### Comparing `acom_music_box-2.1.0/src/acom_music_box/music_box_conditions.py` & `acom_music_box-2.1.1/src/acom_music_box/music_box_conditions.py`

 * *Files 12% similar despite different names*

```diff
@@ -33,21 +33,26 @@
         self.temperature = temperature
         self.species_concentrations = species_concentrations if species_concentrations is not None else []
         self.reaction_rates = reaction_rates if reaction_rates is not None else []
 
     @classmethod
     def from_UI_JSON(cls, UI_JSON, species_list, reaction_list):
         """
-        Create a new instance of the Conditions class from a JSON object.
+        Creates an instance of the class from a UI JSON object.
+
+        This class method takes a UI JSON object, a species list, and a reaction list, 
+        and uses them to create a new instance of the class.
 
         Args:
-            UI_JSON (dict): A JSON object representing the conditions.
+            UI_JSON (dict): The UI JSON object containing the initial conditions and settings.
+            species_list (SpeciesList): A SpeciesList containing the species involved in the simulation.
+            reaction_list (ReactionList): A ReactionList containing the reactions involved in the simulation.
 
         Returns:
-            Conditions: A new instance of the Conditions class.
+            object: An instance of the Conditions class with the settings from the UI JSON object.
         """
         pressure = convert_pressure(UI_JSON['conditions']['environmental conditions']['pressure'], 'initial value')
 
         temperature = convert_temperature(UI_JSON['conditions']['environmental conditions']['temperature'], 'initial value')
 
         # Set initial species concentrations
         species_concentrations = []
@@ -75,14 +80,29 @@
             reaction_rates.append(ReactionRate(reaction_from_list, rate))
            
          
         return cls(pressure, temperature, species_concentrations, reaction_rates)
     
     @classmethod
     def from_config_JSON(cls, path_to_json, config_JSON, species_list, reaction_list):
+        """
+        Creates an instance of the class from a configuration JSON object.
+
+        This class method takes a path to a JSON file, a configuration JSON object, a species list, 
+        and a reaction list, and uses them to create a new instance of the class.
+
+        Args:
+            path_to_json (str): The path to the JSON file containing the initial conditions and settings.
+            config_JSON (dict): The configuration JSON object containing the initial conditions and settings.
+            species_list (SpeciesList): A SpeciesList containing the species involved in the simulation.
+            reaction_list (ReactionList): A ReactionList containing the reactions involved in the simulation.
+
+        Returns:
+            object: An instance of the Conditions class with the settings from the configuration JSON object.
+        """
         pressure = convert_pressure(config_JSON['environmental conditions']['pressure'], 'initial value')
 
         temperature = convert_temperature(config_JSON['environmental conditions']['temperature'], 'initial value')
 
 
         # Set initial species concentrations
         species_concentrations = []
@@ -103,28 +123,39 @@
 
                 species_concentrations.append(SpeciesConcentration(species, concentration))
         
         for species in species_list.species:
             if not any(conc.species.name == species.name for conc in species_concentrations):
                 species_concentrations.append(SpeciesConcentration(species, 0)) 
 
-
-        #TODO: may or may not be necessary
         # Set initial reaction rates
 
         for reaction in reaction_list.reactions:
             if reaction.name != None and not any(reac.reaction.name == reaction.name for reac in reaction_rates):
                 reaction_rates.append(ReactionRate(reaction, 0)) 
 
         
         return cls(pressure, temperature, species_concentrations, reaction_rates)
 
 
     @classmethod
     def read_initial_rates_from_file(cls, file_path, reaction_list):
+        """
+        Reads initial reaction rates from a file.
+
+        This class method takes a file path and a ReactionList, reads the file, and 
+        sets the initial reaction rates based on the contents of the file.
+
+        Args:
+            file_path (str): The path to the file containing the initial reaction rates.
+            reaction_list (ReactionList): A ReactionList containing the reactions involved in the simulation.
+
+        Returns:
+            list: A list where each element represents the initial rate of a reaction.
+        """
 
         reaction_rates = []
 
         with open(file_path, 'r') as csv_file:
             initial_conditions = list(csv.reader(csv_file))
                                       
             if(len(initial_conditions) > 1):
```

### Comparing `acom_music_box-2.1.0/src/acom_music_box/music_box_evolving_conditions.py` & `acom_music_box-2.1.1/src/acom_music_box/music_box_evolving_conditions.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,31 +13,32 @@
     Attributes:
         time (List[float]): A list of time points.
         conditions (List[Conditions]): A list of associated conditions.
     """
 
     def __init__(self, headers=None, times=None, conditions=None):
         """
-        Initializes a new instance of the EvolvingConditions class.
+        Initializes an instance of the EvolvingConditions class.
 
         Args:
-            time (List[float]): A list of time points. Default is an empty list.
-            conditions (List[Conditions]): A list of associated conditions. Default is an empty list.
+            headers (list, optional): A list of headers for the data. Defaults to None.
+            times (list, optional): A list of times at which the conditions are recorded. Defaults to None.
+            conditions (list, optional): A list of conditions at each time point. Defaults to None.
         """
         self.headers = headers if headers is not None else []
         self.times = times if times is not None else []
         self.conditions = conditions if conditions is not None else []
 
     @classmethod
     def from_UI_JSON(cls, UI_JSON, species_list, reaction_list):
         """
         Create a new instance of the EvolvingConditions class from a JSON object.
 
         Args:
-            UI_JSON (dict): A JSON object representing the evolving conditions.
+        UI_JSON (dict): A JSON object representing the evolving conditions.
 
         Returns:
             EvolvingConditions: A new instance of the EvolvingConditions class.
         """
         times = []
         conditions = []
 
@@ -82,16 +83,30 @@
 
             conditions.append(Conditions(pressure, temperature, concentrations, rates))
 
         return cls(headers, times, conditions)
     
     @classmethod
     def from_config_JSON(cls, path_to_json ,config_JSON, species_list, reaction_list):
-        # Initialize empty lists for times and conditions
-        
+        """
+        Creates an instance of the EvolvingConditions class from a configuration JSON object.
+
+        This class method takes a path to a JSON file, a configuration JSON object, a SpeciesList, 
+        and a ReactionList, and uses them to create a new instance of the EvolvingConditions class.
+
+        Args:
+            path_to_json (str): The path to the JSON file containing the initial conditions and settings.
+            config_JSON (dict): The configuration JSON object containing the initial conditions and settings.
+            species_list (SpeciesList): A SpeciesList containing the species involved in the simulation.
+            reaction_list (ReactionList): A ReactionList containing the reactions involved in the simulation.
+
+        Returns:
+            EvolvingConditions: An instance of the EvolvingConditions class with the settings from the configuration JSON object.
+        """
+
 
         evolving_conditions = EvolvingConditions()
         
         # Check if 'evolving conditions' is a key in the JSON config
         if 'evolving conditions' in config_JSON:
             # Construct the path to the evolving conditions file
             evolving_conditions_path = os.path.dirname(path_to_json) + "/" + list(config_JSON['evolving conditions'].keys())[0]
@@ -182,8 +197,18 @@
         # Return a new instance of the class with the times and conditions
         
         return cls(times = times, conditions = conditions)
 
     
     #allows len overload for this class
     def __len__(self):
+        """
+        Returns the number of time points in the EvolvingConditions instance.
+
+        This method is a part of Python's data model methods and allows the built-in 
+        `len()` function to work with an instance of the EvolvingConditions class. 
+        It should return the number of time points for which conditions are recorded.
+
+        Returns:
+            int: The number of time points in the EvolvingConditions instance.
+        """
         return len(self.times)
```

### Comparing `acom_music_box-2.1.0/src/acom_music_box/music_box_model_options.py` & `acom_music_box-2.1.1/src/acom_music_box/music_box_model_options.py`

 * *Files 6% similar despite different names*

```diff
@@ -26,18 +26,18 @@
         self.output_step_time = output_step_time
         self.simulation_length = simulation_length
         self.grid = grid
 
     @classmethod
     def from_UI_JSON(cls, UI_JSON):
         """
-        Create a new instance of the BoxModelOptions class from a JSON object.
+        Create a new instance of the BoxModelOptions class from a JSON object from the MusicBox Interactive UI.
 
         Args:
-            UI_JSON (dict): A JSON object representing the user interface options.
+            UI_JSON (dict): A JSON object representing the box model options from the user interface options.
 
         Returns:
             BoxModelOptions: A new instance of the BoxModelOptions class.
         """
         chem_step_time = convert_time(UI_JSON['conditions']['box model options'], 'chemistry time step') 
         output_step_time = convert_time(UI_JSON['conditions']['box model options'], 'output time step')
         simulation_length = convert_time(UI_JSON['conditions']['box model options'], 'simulation length')
@@ -45,14 +45,23 @@
         grid = UI_JSON['conditions']['box model options']['grid']
         
         return cls(chem_step_time, output_step_time, simulation_length, grid)
     
 
     @classmethod
     def from_config_JSON(cls, config_JSON):
+        """
+        Create a new instance of the BoxModelOptions class from a JSON object from a configuration JSON.
+
+        Args:
+            UI_JSON (dict): A JSON object representing box model options.
+
+        Returns:
+            BoxModelOptions: A new instance of the BoxModelOptions class.
+        """
 
         chem_step_time = convert_time(config_JSON['box model options'], 'chemistry time step')
         output_step_time = convert_time(config_JSON['box model options'], 'output time step') 
         simulation_length = convert_time(config_JSON['box model options'], 'simulation length')
 
         grid = config_JSON['box model options']['grid']
```

### Comparing `acom_music_box-2.1.0/src/acom_music_box/music_box_product.py` & `acom_music_box-2.1.1/src/acom_music_box/music_box_product.py`

 * *Files identical despite different names*

### Comparing `acom_music_box-2.1.0/src/acom_music_box/music_box_reactant.py` & `acom_music_box-2.1.1/src/acom_music_box/music_box_reactant.py`

 * *Files identical despite different names*

### Comparing `acom_music_box-2.1.0/src/acom_music_box/music_box_reaction_rate.py` & `acom_music_box-2.1.1/src/acom_music_box/music_box_reaction_rate.py`

 * *Files identical despite different names*

### Comparing `acom_music_box-2.1.0/src/acom_music_box/music_box_species.py` & `acom_music_box-2.1.1/src/acom_music_box/music_box_species.py`

 * *Files identical despite different names*

### Comparing `acom_music_box-2.1.0/src/acom_music_box/music_box_species_concentration.py` & `acom_music_box-2.1.1/src/acom_music_box/music_box_species_concentration.py`

 * *Files identical despite different names*

### Comparing `acom_music_box-2.1.0/src/acom_music_box/music_box_species_list.py` & `acom_music_box-2.1.1/src/acom_music_box/music_box_species_list.py`

 * *Files 3% similar despite different names*

```diff
@@ -14,26 +14,26 @@
 
     def __init__(self, species=None, relative_tolerance=1.0e-4):
         """
         Initializes a new instance of the SpeciesList class.
 
         Args:
             species (List[Species]): A list of Species instances. Default is an empty list.
-            relative_tolerance (float): The relative tolerance for the species list. Default is 0.0.
+            relative_tolerance (float): The relative tolerance for the species list. Default is 1.0e-4.
         """
         self.species = species if species is not None else []
         self.relative_tolerance = relative_tolerance
 
     @classmethod
     def from_UI_JSON(cls, UI_JSON):
         """
         Create a new instance of the SpeciesList class from a JSON object.
 
         Args:
-            UI_JSON (dict): A JSON object representing the species list.
+            UI_JSON (dict): A JSON object from MusicBox Interactive representing the species list.
 
         Returns:
             SpeciesList: A new instance of the SpeciesList class.
         """
         species_from_json = []
 
         for species in UI_JSON['mechanism']['species']['camp-data']:
@@ -45,14 +45,23 @@
 
             species_from_json.append(Species(name, absolute_tolerance, None, molecular_weight, None))
         
         return cls(species_from_json)
     
     @classmethod
     def from_config_JSON(cls, path_to_json, config_JSON):
+        """
+        Create a new instance of the SpeciesList class from a JSON object.
+
+        Args:
+            UI_JSON (dict): A JSON object from a config JSON representing the species list.
+
+        Returns:
+            SpeciesList: A new instance of the SpeciesList class.
+        """
 
         species_from_json = []
 
         #gets config file path
         config_file_path = os.path.dirname(path_to_json) + "/" + config_JSON['model components'][0]['configuration file']
 
         #opnens config path to read species file
```

### Comparing `acom_music_box-2.1.0/src/acom_music_box/utils.py` & `acom_music_box-2.1.1/src/acom_music_box/utils.py`

 * *Files identical despite different names*

