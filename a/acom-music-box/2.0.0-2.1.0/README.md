# Comparing `tmp/acom_music_box-2.0.0.tar.gz` & `tmp/acom_music_box-2.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "acom_music_box-2.0.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "acom_music_box-2.1.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `acom_music_box-2.0.0.tar` & `acom_music_box-2.1.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0    11357 2023-03-14 22:08:46.581988 acom_music_box-2.0.0/LICENSE
--rw-r--r--   0        0        0      792 2024-02-22 21:23:57.176394 acom_music_box-2.0.0/README.md
--rw-r--r--   0        0        0      414 2024-04-09 15:36:41.773579 acom_music_box-2.0.0/pyproject.toml
--rw-r--r--   0        0        0      858 2024-04-09 15:16:48.180773 acom_music_box-2.0.0/src/acom_music_box/__init__.py
--rw-r--r--   0        0        0    24079 2024-04-09 15:16:48.181627 acom_music_box-2.0.0/src/acom_music_box/music_box.py
--rw-r--r--   0        0        0     8059 2024-04-09 15:16:48.181933 acom_music_box-2.0.0/src/acom_music_box/music_box_conditions.py
--rw-r--r--   0        0        0     8070 2024-04-09 15:16:48.182156 acom_music_box-2.0.0/src/acom_music_box/music_box_evolving_conditions.py
--rw-r--r--   0        0        0     2511 2024-04-09 15:16:48.182332 acom_music_box-2.0.0/src/acom_music_box/music_box_model_options.py
--rw-r--r--   0        0        0      699 2024-04-09 15:16:48.182536 acom_music_box-2.0.0/src/acom_music_box/music_box_product.py
--rw-r--r--   0        0        0      615 2024-04-09 15:16:48.182747 acom_music_box-2.0.0/src/acom_music_box/music_box_reactant.py
--rw-r--r--   0        0        0     3218 2024-04-09 15:16:48.182940 acom_music_box-2.0.0/src/acom_music_box/music_box_reaction.py
--rw-r--r--   0        0        0     6432 2024-04-09 15:16:48.183141 acom_music_box-2.0.0/src/acom_music_box/music_box_reaction_list.py
--rw-r--r--   0        0        0      604 2024-04-09 15:16:48.183329 acom_music_box-2.0.0/src/acom_music_box/music_box_reaction_rate.py
--rw-r--r--   0        0        0     1211 2024-04-09 15:16:48.183543 acom_music_box-2.0.0/src/acom_music_box/music_box_species.py
--rw-r--r--   0        0        0      638 2024-04-09 15:16:48.183736 acom_music_box-2.0.0/src/acom_music_box/music_box_species_concentration.py
--rw-r--r--   0        0        0     3771 2024-04-09 15:16:48.183908 acom_music_box-2.0.0/src/acom_music_box/music_box_species_list.py
--rw-r--r--   0        0        0     3381 2024-04-09 15:16:48.184123 acom_music_box-2.0.0/src/acom_music_box/utils.py
--rw-r--r--   0        0        0     1098 1970-01-01 00:00:00.000000 acom_music_box-2.0.0/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-03-14 22:08:46.581988 acom_music_box-2.1.0/LICENSE
+-rw-r--r--   0        0        0      792 2024-04-09 15:52:10.065732 acom_music_box-2.1.0/README.md
+-rw-r--r--   0        0        0      414 2024-04-09 15:52:10.066098 acom_music_box-2.1.0/pyproject.toml
+-rw-r--r--   0        0        0      858 2024-04-18 13:38:21.379266 acom_music_box-2.1.0/src/acom_music_box/__init__.py
+-rw-r--r--   0        0        0    25087 2024-04-18 13:38:09.354114 acom_music_box-2.1.0/src/acom_music_box/music_box.py
+-rw-r--r--   0        0        0     9227 2024-04-18 13:38:09.354683 acom_music_box-2.1.0/src/acom_music_box/music_box_conditions.py
+-rw-r--r--   0        0        0     8301 2024-04-18 13:38:09.355332 acom_music_box-2.1.0/src/acom_music_box/music_box_evolving_conditions.py
+-rw-r--r--   0        0        0     2511 2024-04-09 15:52:10.067450 acom_music_box-2.1.0/src/acom_music_box/music_box_model_options.py
+-rw-r--r--   0        0        0      699 2024-04-09 15:52:10.067583 acom_music_box-2.1.0/src/acom_music_box/music_box_product.py
+-rw-r--r--   0        0        0      615 2024-04-09 15:52:10.067829 acom_music_box-2.1.0/src/acom_music_box/music_box_reactant.py
+-rw-r--r--   0        0        0     3284 2024-04-18 13:38:09.356246 acom_music_box-2.1.0/src/acom_music_box/music_box_reaction.py
+-rw-r--r--   0        0        0     6542 2024-04-18 13:38:09.356739 acom_music_box-2.1.0/src/acom_music_box/music_box_reaction_list.py
+-rw-r--r--   0        0        0      604 2024-04-09 15:52:10.068265 acom_music_box-2.1.0/src/acom_music_box/music_box_reaction_rate.py
+-rw-r--r--   0        0        0     1211 2024-04-09 15:52:10.068390 acom_music_box-2.1.0/src/acom_music_box/music_box_species.py
+-rw-r--r--   0        0        0      638 2024-04-09 15:52:10.068585 acom_music_box-2.1.0/src/acom_music_box/music_box_species_concentration.py
+-rw-r--r--   0        0        0     3845 2024-04-12 20:15:10.522570 acom_music_box-2.1.0/src/acom_music_box/music_box_species_list.py
+-rw-r--r--   0        0        0     3381 2024-04-09 15:52:10.068879 acom_music_box-2.1.0/src/acom_music_box/utils.py
+-rw-r--r--   0        0        0     1098 1970-01-01 00:00:00.000000 acom_music_box-2.1.0/PKG-INFO
```

### Comparing `acom_music_box-2.0.0/LICENSE` & `acom_music_box-2.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `acom_music_box-2.0.0/README.md` & `acom_music_box-2.1.0/README.md`

 * *Files identical despite different names*

### Comparing `acom_music_box-2.0.0/src/acom_music_box/__init__.py` & `acom_music_box-2.1.0/src/acom_music_box/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """
 This is the music_box package.
 
 This package contains modules for handling various aspects of a music box, 
 including species, products, reactants, reactions, and more.
 """
-__version__ = "2.0.0"
+__version__ = "2.1.0"
 
 from .utils import convert_time, convert_pressure, convert_temperature, convert_concentration
 from .music_box_species import Species
 from .music_box_product import Product
 from .music_box_reactant import Reactant
 from .music_box_reaction import Reaction, Branched, Arrhenius, Tunneling, Troe_Ternary
 from .music_box_species_list import SpeciesList
```

### Comparing `acom_music_box-2.0.0/src/acom_music_box/music_box.py` & `acom_music_box-2.1.0/src/acom_music_box/music_box.py`

 * *Files 2% similar despite different names*

```diff
@@ -114,19 +114,19 @@
                 },
             }
 
             data["evolving conditions"] = {
                 "evolving_conditions.csv": {},
             }
 
-            data["initial conditions"] = {}
+            data["initial conditions"] = {
+                "initial_conditions.csv": {}
+            }
 
-            for reaction_rate in self.initial_conditions.reaction_rates:
-                name = "PHOT." + reaction_rate.reaction.name + ".s-1"
-                data["initial conditions"][name] = reaction_rate.rate
+           
 
             data["model components"] = [
                 {
                     "type": "CAMP",
                     "configuration file": "camp_data/config.json",
                     "override species": {
                         "M": {
@@ -137,14 +137,15 @@
                         "M": {}
                     }
                 }
             ]
 
             config_file.write(json.dumps(data, indent=4))
         
+        
         # Make evolving conditions config
         with open(output_path + "/evolving_conditions.csv", 'w', newline='') as evolving_conditions_file:
             writer = csv.writer(evolving_conditions_file)
             writer.writerow(self.evolving_conditions.headers)
 
             for i in range(len(self.evolving_conditions.times)):
                 row = [self.evolving_conditions.times[i]]
@@ -167,30 +168,53 @@
                             reaction_name = reaction_name[1]
 
                         reaction_rate = next((x for x in self.evolving_conditions.conditions[i].reaction_rates if x.reaction.name == reaction_name), None)
                         row.append(reaction_rate.rate) 
 
                 writer.writerow(row)
 
+
+
+        reaction_names = []
+        reaction_rates = []
+
+        for reaction_rate in self.initial_conditions.reaction_rates:
+            if reaction_rate.reaction.reaction_type == "PHOTOLYSIS":
+                name = "PHOT." + reaction_rate.reaction.name + ".s-1"
+            elif reaction_rate.reaction.reaction_type == "LOSS":
+                name = "LOSS." + reaction_rate.reaction.name + ".s-1"
+            elif reaction_rate.reaction.reaction_type == "EMISSION":
+                name = "EMISSION." + reaction_rate.reaction.name + ".s-1"
+
+            reaction_names.append(name)
+            reaction_rates.append(reaction_rate.rate)
+        #writes reaction rates inital conditions to file
+        with open(output_path + "/initial_conditions.csv", 'w', newline='') as initial_conditions_file:
+            writer = csv.writer(initial_conditions_file)
+            writer.writerow(reaction_names)
+            writer.writerow(reaction_rates)
+
+
+
     def generateSpeciesConfig(self):
         """
         Generate a JSON configuration for the species in the box model.
 
         Returns:
             str: A JSON-formatted string representing the species configuration.
         """
 
         speciesArray = []
 
         #Adds relative tolerance if value is set
-        # if(self.species_list.relative_tolerance != None):
-        #     relativeTolerance = {}
-        #     relativeTolerance["Type"] = "RELATIVE_TOLERANCE"
-        #     relativeTolerance["value"] = self.species_list.relative_tolerance
-        #     speciesArray.append(relativeTolerance)
+        if(self.species_list.relative_tolerance != None):
+            relativeTolerance = {}
+            relativeTolerance["type"] = "RELATIVE_TOLERANCE"
+            relativeTolerance["value"] = self.species_list.relative_tolerance
+            speciesArray.append(relativeTolerance)
 
         #Adds species to config
         for species in self.species_list.species:
             spec = {}
 
             #Add species name if value is set
             if(species.name != None):
@@ -354,14 +378,17 @@
                 if reaction.N is not None:
                     reac["N"] = reaction.N
             
             #Adds reaction name if value is set
             if(reaction.name != None):
                 reac["MUSICA name"] = reaction.name
 
+            if(reaction.scaling_factor != None):
+                reac["scaling factor"] = reaction.scaling_factor
+
             reactionsArray.append(reac)
 
         reacList["reactions"] = reactionsArray
 
         reactionsJson = {
             "camp-data" : [reacList]
         }
@@ -416,22 +443,24 @@
         headers = []
         headers.append("time")
         headers.append("ENV.temperature")
         headers.append("ENV.pressure")
 
         rate_constant_ordering = musica.user_defined_reaction_rates(self.solver)
         species_constant_ordering = musica.species_ordering(self.solver)
+  
         
         #adds species headers to output
         ordered_species_headers =  [k for k, v in sorted(species_constant_ordering.items(), key=lambda item: item[1])]
         for spec in ordered_species_headers:
             headers.append("CONC." + spec)
 
         ordered_concentrations = self.order_species_concentrations(curr_conditions, species_constant_ordering)
         ordered_rate_constants = self.order_reaction_rates(curr_conditions, rate_constant_ordering)
+   
         
         output_array.append(headers)
         
         
         curr_time = 0
         next_output_time = curr_time
         #runs the simulation at each timestep
@@ -449,36 +478,38 @@
                     row.append(conc)
                 output_array.append(row)
                 next_output_time += self.box_model_options.output_step_time
         
             #iterates evolvings conditons if enough time has elapsed
             while(next_conditions != None and next_conditions_time <= curr_time):
                
-                #curr_conditions = next_conditions
                 curr_conditions.update_conditions(next_conditions)
                 
-
                 #iterates next_conditions if there are remaining evolving conditions
                 if(len(self.evolving_conditions) > next_conditions_index + 1):
                     next_conditions_index += 1
                     next_conditions = self.evolving_conditions.conditions[next_conditions_index]
                     next_conditions_time = self.evolving_conditions.times[next_conditions_index]
-
-                   
-                    #overrides concentrations if specified by conditions
-                    if(len(curr_conditions.get_concentration_array()) != 0):
-                        ordered_concentrations = self.order_species_concentrations(curr_conditions, species_constant_ordering)
                     
                     ordered_rate_constants = self.order_reaction_rates(curr_conditions, rate_constant_ordering)
                     
                 else:
                     next_conditions = None
             
+            
+            #updates M accordingly
+            if 'M' in species_constant_ordering:
+                BOLTZMANN_CONSTANT = 1.380649e-23
+                AVOGADRO_CONSTANT = 6.02214076e23;  
+                GAS_CONSTANT = BOLTZMANN_CONSTANT * AVOGADRO_CONSTANT
+                ordered_concentrations[species_constant_ordering['M']] = curr_conditions.pressure / (GAS_CONSTANT * curr_conditions.temperature)
+
             #solves and updates concentration values in concentration array
             musica.micm_solve(self.solver, self.box_model_options.chem_step_time, curr_conditions.temperature, curr_conditions.pressure, ordered_concentrations, ordered_rate_constants)
+
            
 
         
             #increments time
             curr_time += self.box_model_options.chem_step_time  
         
         #outputs to file if output is present
@@ -544,15 +575,15 @@
 
             # Set species list
             self.species_list = SpeciesList.from_config_JSON(path_to_json, data)
 
             self.reaction_list = ReactionList.from_config_JSON(path_to_json, data, self.species_list)
 
             # Set initial conditions
-            self.initial_conditions = Conditions.from_config_JSON(data, self.species_list, self.reaction_list)
+            self.initial_conditions = Conditions.from_config_JSON(path_to_json, data, self.species_list, self.reaction_list)
 
             # Set initial conditions
             self.evolving_conditions = EvolvingConditions.from_config_JSON(path_to_json, data, self.species_list, self.reaction_list)
             
 
     def speciesOrdering(self):
         return musica.species_ordering(self.solver)
@@ -578,18 +609,18 @@
 
             ordered_rate_constants[rate_constant_ordering[key]] = float(value)
         return ordered_rate_constants
     
     @classmethod
     def order_species_concentrations(self, curr_conditions, species_constant_ordering):
         concentrations = {}
+
         for concentraton in curr_conditions.species_concentrations:
             concentrations[concentraton.species.name] = concentraton.concentration
             
         ordered_concentrations = len(concentrations.keys()) * [0.0]
         
         for key, value in concentrations.items():
-
             ordered_concentrations[species_constant_ordering[key]] = value
         return ordered_concentrations
```

### Comparing `acom_music_box-2.0.0/src/acom_music_box/music_box_conditions.py` & `acom_music_box-2.1.0/src/acom_music_box/music_box_conditions.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+import csv
+import os
 from typing import List
 from .music_box_reaction_rate import ReactionRate
 from .music_box_species import Species
 from .music_box_species_concentration import SpeciesConcentration
 from .utils import convert_time, convert_pressure, convert_temperature, convert_concentration
 
 
@@ -72,28 +74,31 @@
 
             reaction_rates.append(ReactionRate(reaction_from_list, rate))
            
          
         return cls(pressure, temperature, species_concentrations, reaction_rates)
     
     @classmethod
-    def from_config_JSON(cls, config_JSON, species_list, reaction_list):
+    def from_config_JSON(cls, path_to_json, config_JSON, species_list, reaction_list):
         pressure = convert_pressure(config_JSON['environmental conditions']['pressure'], 'initial value')
 
         temperature = convert_temperature(config_JSON['environmental conditions']['temperature'], 'initial value')
 
 
         # Set initial species concentrations
         species_concentrations = []
+        reaction_rates = []
 
         #reads initial conditions from csv if it is given
-        if 'initial conditions' in config_JSON:
-            initial_conditions_csv = config_JSON['initial conditions']
-            #read_initial_conditions_from_csv(initial_conditions_csv)
+        if 'initial conditions' in config_JSON and len(list(config_JSON['initial conditions'].keys())) > 0:
+
+            initial_conditions_path = os.path.dirname(path_to_json) + "/" + list(config_JSON['initial conditions'].keys())[0]
+            reaction_rates = Conditions.read_initial_rates_from_file(initial_conditions_path, reaction_list)
 
+            
         #reads from config file directly if present
         if 'chemical species' in config_JSON:
             for chem_spec in config_JSON['chemical species']:
                 species = Species(name = chem_spec)
                 concentration = convert_concentration(config_JSON['chemical species'][chem_spec], 'initial value')
 
                 species_concentrations.append(SpeciesConcentration(species, concentration))
@@ -101,24 +106,52 @@
         for species in species_list.species:
             if not any(conc.species.name == species.name for conc in species_concentrations):
                 species_concentrations.append(SpeciesConcentration(species, 0)) 
 
 
         #TODO: may or may not be necessary
         # Set initial reaction rates
-        reaction_rates = []
 
         for reaction in reaction_list.reactions:
             if reaction.name != None and not any(reac.reaction.name == reaction.name for reac in reaction_rates):
                 reaction_rates.append(ReactionRate(reaction, 0)) 
 
-
+        
         return cls(pressure, temperature, species_concentrations, reaction_rates)
 
 
+    @classmethod
+    def read_initial_rates_from_file(cls, file_path, reaction_list):
+
+        reaction_rates = []
+
+        with open(file_path, 'r') as csv_file:
+            initial_conditions = list(csv.reader(csv_file))
+                                      
+            if(len(initial_conditions) > 1):
+                # The first row of the CSV contains headers
+                headers = initial_conditions[0]
+
+                # The second row of the CSV contains rates
+                rates = initial_conditions[1]
+
+                
+                for i in range(0, len(headers)):
+
+
+                    reaction_rate = headers[i]
+
+                    match = filter(lambda x: x.name == reaction_rate.split('.')[1], reaction_list.reactions)
+                    
+                    reaction = next(match, None)
+                    rate = rates[i]
+
+                    reaction_rates.append(ReactionRate(reaction, rate))
+        return reaction_rates
+
 
     def add_species_concentration(self, species_concentration):
         """
         Add a SpeciesConcentration instance to the list of species concentrations.
 
         Args:
             species_concentration (SpeciesConcentration): The SpeciesConcentration instance to be added.
```

### Comparing `acom_music_box-2.0.0/src/acom_music_box/music_box_evolving_conditions.py` & `acom_music_box-2.1.0/src/acom_music_box/music_box_evolving_conditions.py`

 * *Files 1% similar despite different names*

```diff
@@ -121,66 +121,67 @@
         """
 
         times = []
         conditions = []
         
         # Open the evolving conditions file and read it as a CSV
         with open(file_path, 'r') as csv_file:
-            evolving_conditions = list(csv.reader(csv_file))
-
-            # The first row of the CSV contains headers
-            headers = evolving_conditions[0]
+            evolving_conditions = list(csv.reader(csv_file)) 
             
-            # Iterate over the remaining rows of the CSV
-            for i in range(1, len(evolving_conditions)):
-                # The first column of each row is a time value
-                times.append(float(evolving_conditions[i][0]))
-
-                # Initialize pressure and temperature as None
-                pressure = None
-                temperature = None
-
-                # If pressure and temperature headers are present in the CSV, extract their values
-                if 'ENV.pressure.Pa' in headers:
-                    pressure = float(evolving_conditions[i][headers.index('ENV.pressure.Pa')])
-                if 'ENV.temperature.K' in headers:
-                    temperature = float(evolving_conditions[i][headers.index('ENV.temperature.K')])
-
-                # Initialize concentrations list and extract concentration headers
-                concentrations = []
-                concentration_headers = list(filter(lambda x: 'CONC' in x, headers))
-
-                # For each concentration header, find the matching species and append its concentration to the list
-                for j in range(len(concentration_headers)):
-                    match = filter(lambda x: x.name == concentration_headers[j].split('.')[1], species_list.species)
-                    species = next(match, None)
-                    concentration = float(evolving_conditions[i][headers.index(concentration_headers[j])])
-                    
-                    concentrations.append(SpeciesConcentration(species, concentration))
-                    
-
-                # Initialize rates list and extract rate headers
-                rates = []
-                rate_headers = list(filter(lambda x: 's-1' in x, headers))
-
-                # For each rate header, find the matching reaction and append its rate to the list
-                for k in range(len(rate_headers)):
-                    name_to_match = rate_headers[k].split('.')
-                    
-                    if name_to_match[0] == 'LOSS' or name_to_match[0] == 'EMIS':
-                        name_to_match = name_to_match[0] + '_' + name_to_match[1]
-                    else:
-                        name_to_match = name_to_match[1]
-                    match = filter(lambda x: x.name == name_to_match, reaction_list.reactions)
-                    reaction = next(match, None)
-                    rate = float(evolving_conditions[i][headers.index(rate_headers[k])])
-                    rates.append(ReactionRate(reaction, rate))
+            if(len(evolving_conditions) > 1):
+                # The first row of the CSV contains headers
+                headers = evolving_conditions[0]
+                
+                # Iterate over the remaining rows of the CSV
+                for i in range(1, len(evolving_conditions)):
+                    # The first column of each row is a time value
+                    times.append(float(evolving_conditions[i][0]))
+
+                    # Initialize pressure and temperature as None
+                    pressure = None
+                    temperature = None
+
+                    # If pressure and temperature headers are present in the CSV, extract their values
+                    if 'ENV.pressure.Pa' in headers:
+                        pressure = float(evolving_conditions[i][headers.index('ENV.pressure.Pa')])
+                    if 'ENV.temperature.K' in headers:
+                        temperature = float(evolving_conditions[i][headers.index('ENV.temperature.K')])
+
+                    # Initialize concentrations list and extract concentration headers
+                    concentrations = []
+                    concentration_headers = list(filter(lambda x: 'CONC' in x, headers))
+
+                    # For each concentration header, find the matching species and append its concentration to the list
+                    for j in range(len(concentration_headers)):
+                        match = filter(lambda x: x.name == concentration_headers[j].split('.')[1], species_list.species)
+                        species = next(match, None)
+                        concentration = float(evolving_conditions[i][headers.index(concentration_headers[j])])
+                        
+                        concentrations.append(SpeciesConcentration(species, concentration))
+                        
+
+                    # Initialize rates list and extract rate headers
+                    rates = []
+                    rate_headers = list(filter(lambda x: 's-1' in x, headers))
+
+                    # For each rate header, find the matching reaction and append its rate to the list
+                    for k in range(len(rate_headers)):
+                        name_to_match = rate_headers[k].split('.')
+                        
+                        if name_to_match[0] == 'LOSS' or name_to_match[0] == 'EMIS':
+                            name_to_match = name_to_match[0] + '_' + name_to_match[1]
+                        else:
+                            name_to_match = name_to_match[1]
+                        match = filter(lambda x: x.name == name_to_match, reaction_list.reactions)
+                        reaction = next(match, None)
+                        rate = float(evolving_conditions[i][headers.index(rate_headers[k])])
+                        rates.append(ReactionRate(reaction, rate))
 
-                # Append the conditions for this time point to the conditions list
-                conditions.append(Conditions(pressure, temperature, concentrations, rates))
+                    # Append the conditions for this time point to the conditions list
+                    conditions.append(Conditions(pressure, temperature, concentrations, rates))
 
         # Return a new instance of the class with the times and conditions
         
         return cls(times = times, conditions = conditions)
 
     
     #allows len overload for this class
```

### Comparing `acom_music_box-2.0.0/src/acom_music_box/music_box_model_options.py` & `acom_music_box-2.1.0/src/acom_music_box/music_box_model_options.py`

 * *Files identical despite different names*

### Comparing `acom_music_box-2.0.0/src/acom_music_box/music_box_product.py` & `acom_music_box-2.1.0/src/acom_music_box/music_box_product.py`

 * *Files identical despite different names*

### Comparing `acom_music_box-2.0.0/src/acom_music_box/music_box_reactant.py` & `acom_music_box-2.1.0/src/acom_music_box/music_box_reactant.py`

 * *Files identical despite different names*

### Comparing `acom_music_box-2.0.0/src/acom_music_box/music_box_reaction.py` & `acom_music_box-2.1.0/src/acom_music_box/music_box_reaction.py`

 * *Files 8% similar despite different names*

```diff
@@ -7,28 +7,29 @@
     Attributes:
         name (str): The name of the reaction.
         reaction_type (str): The type of the reaction.
         reactants (List[Reactant]): A list of Reactant instances representing the reactants. Default is an empty list.
         products (List[Product]): A list of Product instances representing the products. Default is an empty list.
     """
 
-    def __init__(self, name=None, reaction_type=None, reactants=None, products=None):
+    def __init__(self, name=None, reaction_type=None, reactants=None, products=None, scaling_factor=None):
         """
         Initializes a new instance of the Reaction class.
 
         Args:
             name (str): The name of the reaction.
             reaction_type (str): The type of the reaction.
             reactants (List[Reactant]): A list of Reactant instances representing the reactants. Default is an empty list.
             products (List[Product]): A list of Product instances representing the products. Default is an empty list.
         """
         self.name = name
         self.reaction_type = reaction_type
         self.reactants = reactants if reactants is not None else []
         self.products = products if products is not None else []
+        self.scaling_factor = scaling_factor
 
     def add_reactant(self, reactant):
         """
         Add a Reactant instance to the list of reactants.
 
         Args:
             reactant (Reactant): The Reactant instance to be added.
```

### Comparing `acom_music_box-2.0.0/src/acom_music_box/music_box_reaction_list.py` & `acom_music_box-2.1.0/src/acom_music_box/music_box_reaction_list.py`

 * *Files 4% similar despite different names*

```diff
@@ -107,14 +107,15 @@
                     products.append(Product(species, yield_value))
         return products
     
     @classmethod
     def get_reactions_from_JSON(self, reaction, species_list):
 
         name = reaction['MUSICA name'] if 'MUSICA name' in reaction else None
+        scaling_factor = reaction['scaling factor'] if 'scaling factor' in reaction else None
         reaction_type = reaction['type']
     
         reactants = ReactionList.get_reactants_from_JSON(reaction, species_list)
         products = ReactionList.get_products_from_JSON(reaction, species_list)
                 
         if reaction_type == 'WENNBERG_NO_RO2':
             alkoxy_products = []
@@ -159,8 +160,8 @@
             kinf_A = reaction.get('kinf_A')
             kinf_B = reaction.get('kinf_B')
             kinf_C = reaction.get('kinf_C')
             Fc = reaction.get('Fc')
             N = reaction.get('N')
             return Troe_Ternary(name, reaction_type, reactants, products, k0_A, k0_B, k0_C, kinf_A, kinf_B, kinf_C, Fc, N)
         else:
-            return Reaction(name, reaction_type, reactants, products)
+            return Reaction(name, reaction_type, reactants, products, scaling_factor)
```

### Comparing `acom_music_box-2.0.0/src/acom_music_box/music_box_reaction_rate.py` & `acom_music_box-2.1.0/src/acom_music_box/music_box_reaction_rate.py`

 * *Files identical despite different names*

### Comparing `acom_music_box-2.0.0/src/acom_music_box/music_box_species.py` & `acom_music_box-2.1.0/src/acom_music_box/music_box_species.py`

 * *Files identical despite different names*

### Comparing `acom_music_box-2.0.0/src/acom_music_box/music_box_species_concentration.py` & `acom_music_box-2.1.0/src/acom_music_box/music_box_species_concentration.py`

 * *Files identical despite different names*

### Comparing `acom_music_box-2.0.0/src/acom_music_box/music_box_species_list.py` & `acom_music_box-2.1.0/src/acom_music_box/music_box_species_list.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     Represents a list of species with a relative tolerance.
 
     Attributes:
         species (List[Species]): A list of Species instances.
         relativeTolerance (float): The relative tolerance for the species list.
     """
 
-    def __init__(self, species=None, relative_tolerance=0.0):
+    def __init__(self, species=None, relative_tolerance=1.0e-4):
         """
         Initializes a new instance of the SpeciesList class.
 
         Args:
             species (List[Species]): A list of Species instances. Default is an empty list.
             relative_tolerance (float): The relative tolerance for the species list. Default is 0.0.
         """
@@ -62,16 +62,17 @@
             #assumes species file is first in the list
             if(len(config['camp-files']) > 0):
                 species_file_path = os.path.dirname(config_file_path) + "/" + config['camp-files'][0]
                 with open(species_file_path, 'r') as species_file:
                     species_data = json.load(species_file)
                     #loads species by names from camp files
                     for properties in species_data['camp-data']:
-                        name = properties.get('name')
-                        species_from_json.append(Species(name, None, None, None, None))
+                        if properties.get('name') is not None:
+                            name = properties.get('name')
+                            species_from_json.append(Species(name, None, None, None, None))
 
 
         #chceks if species are in the config file and updates attributes accordingly
         for chem_spec in config_JSON['chemical species']:
             for species in species_from_json:
                 if species.name == chem_spec:
                     # Add attributes to species
```

### Comparing `acom_music_box-2.0.0/src/acom_music_box/utils.py` & `acom_music_box-2.1.0/src/acom_music_box/utils.py`

 * *Files identical despite different names*

### Comparing `acom_music_box-2.0.0/PKG-INFO` & `acom_music_box-2.1.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: acom_music_box
-Version: 2.0.0
+Version: 2.1.0
 Summary: This is the music_box package.
 Author-email: NCAR/ACOM <musica-support@ucar.edu>
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: Apache Software License
 Project-URL: Home, https://github.com/NCAR/music-box
```

