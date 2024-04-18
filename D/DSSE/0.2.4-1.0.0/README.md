# Comparing `tmp/DSSE-0.2.4.tar.gz` & `tmp/dsse-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "DSSE-0.2.4.tar", last modified: Tue Mar 12 18:39:54 2024, max compression
+gzip compressed data, was "dsse-1.0.0.tar", last modified: Thu Apr 18 19:11:26 2024, max compression
```

## Comparing `DSSE-0.2.4.tar` & `dsse-1.0.0.tar`

### file list

```diff
@@ -1,28 +1,36 @@
-drwxrwxr-x   0 ricardo   (1000) ricardo   (1000)        0 2024-03-12 18:39:54.782095 DSSE-0.2.4/
-drwxrwxr-x   0 ricardo   (1000) ricardo   (1000)        0 2024-03-12 18:39:54.778095 DSSE-0.2.4/DSSE/
--rw-rw-r--   0 ricardo   (1000) ricardo   (1000)      222 2024-03-12 14:40:14.000000 DSSE-0.2.4/DSSE/__init__.py
-drwxrwxr-x   0 ricardo   (1000) ricardo   (1000)        0 2024-03-12 18:39:54.782095 DSSE-0.2.4/DSSE/environment/
--rw-rw-r--   0 ricardo   (1000) ricardo   (1000)        0 2024-03-12 14:40:14.000000 DSSE-0.2.4/DSSE/environment/__init__.py
--rw-rw-r--   0 ricardo   (1000) ricardo   (1000)      256 2024-03-12 14:40:14.000000 DSSE-0.2.4/DSSE/environment/constants.py
--rw-rw-r--   0 ricardo   (1000) ricardo   (1000)    14099 2024-03-12 17:33:18.000000 DSSE-0.2.4/DSSE/environment/env.py
-drwxrwxr-x   0 ricardo   (1000) ricardo   (1000)        0 2024-03-12 18:39:54.782095 DSSE-0.2.4/DSSE/environment/generator/
--rw-rw-r--   0 ricardo   (1000) ricardo   (1000)        0 2024-03-12 14:40:14.000000 DSSE-0.2.4/DSSE/environment/generator/__init__.py
--rw-rw-r--   0 ricardo   (1000) ricardo   (1000)      348 2024-03-12 17:31:43.000000 DSSE-0.2.4/DSSE/environment/generator/circle.py
--rw-rw-r--   0 ricardo   (1000) ricardo   (1000)     5394 2024-03-12 17:31:43.000000 DSSE-0.2.4/DSSE/environment/generator/dynamic_probability.py
--rw-rw-r--   0 ricardo   (1000) ricardo   (1000)     2651 2024-03-12 14:40:14.000000 DSSE-0.2.4/DSSE/environment/generator/person_movement.py
-drwxrwxr-x   0 ricardo   (1000) ricardo   (1000)        0 2024-03-12 18:39:54.782095 DSSE-0.2.4/DSSE/environment/imgs/
--rw-rw-r--   0 ricardo   (1000) ricardo   (1000)        0 2024-03-12 18:38:11.000000 DSSE-0.2.4/DSSE/environment/imgs/__init__.py
--rw-rw-r--   0 ricardo   (1000) ricardo   (1000)    14774 2024-03-12 14:40:14.000000 DSSE-0.2.4/DSSE/environment/imgs/drone.png
--rw-rw-r--   0 ricardo   (1000) ricardo   (1000)    13193 2024-03-12 14:40:14.000000 DSSE-0.2.4/DSSE/environment/imgs/person-swimming.png
--rw-rw-r--   0 ricardo   (1000) ricardo   (1000)     4447 2024-03-12 14:40:14.000000 DSSE-0.2.4/DSSE/environment/pygame_interface.py
-drwxrwxr-x   0 ricardo   (1000) ricardo   (1000)        0 2024-03-12 18:39:54.782095 DSSE-0.2.4/DSSE.egg-info/
--rw-rw-r--   0 ricardo   (1000) ricardo   (1000)    15400 2024-03-12 18:39:54.000000 DSSE-0.2.4/DSSE.egg-info/PKG-INFO
--rw-rw-r--   0 ricardo   (1000) ricardo   (1000)      586 2024-03-12 18:39:54.000000 DSSE-0.2.4/DSSE.egg-info/SOURCES.txt
--rw-rw-r--   0 ricardo   (1000) ricardo   (1000)        1 2024-03-12 18:39:54.000000 DSSE-0.2.4/DSSE.egg-info/dependency_links.txt
--rw-rw-r--   0 ricardo   (1000) ricardo   (1000)       51 2024-03-12 18:39:54.000000 DSSE-0.2.4/DSSE.egg-info/requires.txt
--rw-rw-r--   0 ricardo   (1000) ricardo   (1000)        5 2024-03-12 18:39:54.000000 DSSE-0.2.4/DSSE.egg-info/top_level.txt
--rw-rw-r--   0 ricardo   (1000) ricardo   (1000)       15 2024-03-12 14:40:14.000000 DSSE-0.2.4/MANIFEST.in
--rw-rw-r--   0 ricardo   (1000) ricardo   (1000)    15400 2024-03-12 18:39:54.782095 DSSE-0.2.4/PKG-INFO
--rw-rw-r--   0 ricardo   (1000) ricardo   (1000)    14768 2024-03-12 14:40:14.000000 DSSE-0.2.4/README.md
--rw-rw-r--   0 ricardo   (1000) ricardo   (1000)       38 2024-03-12 18:39:54.782095 DSSE-0.2.4/setup.cfg
--rw-rw-r--   0 ricardo   (1000) ricardo   (1000)     1227 2024-03-12 18:39:50.000000 DSSE-0.2.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 19:11:26.608315 dsse-1.0.0/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 19:11:26.604315 dsse-1.0.0/DSSE/
+-rw-r--r--   0 runner    (1001) docker     (127)      322 2024-04-18 19:11:18.000000 dsse-1.0.0/DSSE/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 19:11:26.604315 dsse-1.0.0/DSSE/environment/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 19:11:18.000000 dsse-1.0.0/DSSE/environment/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      490 2024-04-18 19:11:18.000000 dsse-1.0.0/DSSE/environment/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6333 2024-04-18 19:11:18.000000 dsse-1.0.0/DSSE/environment/coverage_env.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13098 2024-04-18 19:11:18.000000 dsse-1.0.0/DSSE/environment/env.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9359 2024-04-18 19:11:18.000000 dsse-1.0.0/DSSE/environment/env_base.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 19:11:26.604315 dsse-1.0.0/DSSE/environment/imgs/
+-rw-r--r--   0 runner    (1001) docker     (127)    14774 2024-04-18 19:11:18.000000 dsse-1.0.0/DSSE/environment/imgs/drone.png
+-rw-r--r--   0 runner    (1001) docker     (127)    13193 2024-04-18 19:11:18.000000 dsse-1.0.0/DSSE/environment/imgs/person-swimming.png
+-rw-r--r--   0 runner    (1001) docker     (127)     4765 2024-04-18 19:11:18.000000 dsse-1.0.0/DSSE/environment/pygame_interface.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 19:11:26.604315 dsse-1.0.0/DSSE/environment/simulation/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 19:11:18.000000 dsse-1.0.0/DSSE/environment/simulation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4890 2024-04-18 19:11:18.000000 dsse-1.0.0/DSSE/environment/simulation/dynamic_probability.py
+-rw-r--r--   0 runner    (1001) docker     (127)      615 2024-04-18 19:11:18.000000 dsse-1.0.0/DSSE/environment/simulation/particle_sim.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1205 2024-04-18 19:11:18.000000 dsse-1.0.0/DSSE/environment/simulation/time_step.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 19:11:26.608315 dsse-1.0.0/DSSE/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 19:11:18.000000 dsse-1.0.0/DSSE/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1488 2024-04-18 19:11:18.000000 dsse-1.0.0/DSSE/tests/drone_policy.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12802 2024-04-18 19:11:18.000000 dsse-1.0.0/DSSE/tests/test_env.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6193 2024-04-18 19:11:18.000000 dsse-1.0.0/DSSE/tests/test_env_coverage.py
+-rw-r--r--   0 runner    (1001) docker     (127)      581 2024-04-18 19:11:18.000000 dsse-1.0.0/DSSE/tests/test_matrix.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 19:11:26.608315 dsse-1.0.0/DSSE.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    15973 2024-04-18 19:11:26.000000 dsse-1.0.0/DSSE.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      757 2024-04-18 19:11:26.000000 dsse-1.0.0/DSSE.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-18 19:11:26.000000 dsse-1.0.0/DSSE.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-04-18 19:11:26.000000 dsse-1.0.0/DSSE.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-04-18 19:11:26.000000 dsse-1.0.0/DSSE.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1094 2024-04-18 19:11:18.000000 dsse-1.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-18 19:11:18.000000 dsse-1.0.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    15973 2024-04-18 19:11:26.608315 dsse-1.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    15170 2024-04-18 19:11:18.000000 dsse-1.0.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-18 19:11:26.608315 dsse-1.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1164 2024-04-18 19:11:26.000000 dsse-1.0.0/setup.py
```

### Comparing `DSSE-0.2.4/DSSE/environment/env.py` & `dsse-1.0.0/DSSE/environment/env.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,364 +1,353 @@
-from random import random
+from random import random, randint
 import functools
-from copy import copy
 import numpy as np
-from gymnasium.spaces import MultiDiscrete
-from pettingzoo.utils.env import ParallelEnv
-from .generator.person_movement import update_shipwrecked_position, noise_person_movement
-from .generator.dynamic_probability import ProbabilityMatrix
-from .constants import RED, GREEN, Actions
-from .pygame_interface import PygameInterface
+from gymnasium.spaces import MultiDiscrete, Discrete, Box, Tuple
+from .constants import RED, GREEN, Actions, Reward
+from .entities.person import Person
+from .env_base import DroneSwarmSearchBase
 
 
-class DroneSwarmSearch(ParallelEnv):
+class DroneSwarmSearch(DroneSwarmSearchBase):
     """
     PettingZoo based environment for SAR missions using drones.
     """
 
+    possible_actions = {action for action in Actions}
+    metadata = {
+        "name": "DroneSwarmSearchV0",
+    }
+
+    reward_scheme = Reward(
+        default=1,
+        leave_grid=-100_000,
+        exceed_timestep=-100_000,
+        drones_collision=-100_000,
+        search_cell=1,
+        search_and_find=100_000,
+    )
+
     def __init__(
         self,
-        grid_size=7,
+        grid_size=20,
         render_mode="ansi",
         render_grid=False,
         render_gradient=True,
-        n_drones=1,
-        vector=(-0.5, -0.5),
-        person_initial_position=(0, 0),
-        disperse_constant=10,
+        vector=(1.1, 1),
+        dispersion_inc=0.1,
+        dispersion_start=0.5,
         timestep_limit=100,
-        probability_of_detection=1.0,
+        person_amount=1,
+        person_initial_position=(0, 0),
+        drone_amount=1,
+        drone_speed=10,
+        probability_of_detection=1,
+        pre_render_time=0,
     ):
-        self.grid_size = grid_size
-        self._was_reset = False
-
-        # Error Checking
-        if n_drones > grid_size * grid_size:
-            raise ValueError(
-                "There are more drones than grid spots. Reduce number of drones or increase grid size."
-            )
-        if not self.is_valid_position(person_initial_position):
-            raise ValueError("Person initial position is out of the matrix")
-
-        if render_mode != "ansi" and render_mode != "human":
-            raise ValueError("Render mode not recognized")
+        if person_amount <= 0:
+            raise ValueError("The number of persons must be greater than 0.")
+        self.person_amount = person_amount
+
+        super().__init__(
+            grid_size=grid_size,
+            render_mode=render_mode,
+            render_grid=render_grid,
+            render_gradient=render_gradient,
+            vector=vector,
+            dispersion_inc=dispersion_inc,
+            dispersion_start=dispersion_start,
+            timestep_limit=timestep_limit,
+            disaster_position=person_initial_position,
+            drone_amount=drone_amount,
+            drone_speed=drone_speed,
+            probability_of_detection=probability_of_detection,
+            pre_render_time=pre_render_time,
+        )
 
+        # Person initialization
         self.person_initial_position = person_initial_position
-        self.person_y = person_initial_position[1]
-        self.person_x = person_initial_position[0]
-        self.timestep = None
-        self.timestep_limit = timestep_limit
-        self.disperse_constant = disperse_constant
-        self.vector = vector
-        self.possible_agents = []
-        self.agents_positions = {}
-
-        for i in range(n_drones):
-            self.possible_agents.append("drone" + str(i))
-            self.agents_positions["drone" + str(i)] = (None, None)
-
-        self.render_mode = render_mode
-        self.probability_matrix = None
+        self.persons_set = self.create_persons_set()
 
         # Initializing render
-        self.pygame_renderer = PygameInterface(self.grid_size, render_gradient, render_grid)
         self.rewards_sum = {a: 0 for a in self.possible_agents}
         self.rewards_sum["total"] = 0
 
-        self.pod = probability_of_detection
-
-        # Reward Function
-        self.reward_scheme = {
-            "default": 1,
-            "leave_grid": -100000,
-            "exceed_timestep": -100000,
-            "drones_collision": -100000,
-            "search_cell": 1,
-            "search_and_find": 100000,
+        # Define the action and observation spaces for compatibility with RL libraries
+        self.action_spaces = {
+            agent: self.action_space(agent) for agent in self.possible_agents
         }
-    
-    def is_valid_position(self, position: tuple[int, int]) -> bool:
-        valid_x = position[0] >= 0 and position[0] < self.grid_size
-        valid_y = position[1] >= 0 and position[1] < self.grid_size
-        return valid_x and valid_y
-
-
-    def default_drones_positions(self):
-        counter_x = 0
-        counter_y = 0
-        for agent in self.agents:
-            if counter_x >= self.grid_size:
-                counter_x = 0
-                counter_y += 1
-            self.agents_positions[agent] = (counter_x, counter_y)
-            counter_x += 1
+        self.observation_spaces = {
+            agent: self.observation_space(agent) for agent in self.possible_agents
+        }
+
+    def create_persons_set(self) -> set[Person]:
+        persons_set = set()
+        position = self.create_random_positions_person(
+            self.person_initial_position, self.person_amount
+        )
 
-    def required_drone_positions(self, drones_positions: list):
-        if len(drones_positions) != len(self.possible_agents):
+        for i in range(self.person_amount):
+            person = Person(
+                index=i,
+                initial_position=position[i],
+                grid_size=self.grid_size,
+            )
+            person.calculate_movement_vector(self.vector)
+            persons_set.add(person)
+
+            if not self.is_valid_position(person.initial_position):
+                raise ValueError("Person initial position is out of the matrix")
+
+        return persons_set
+
+    def create_random_positions_person(
+        self, central_position: tuple[int, int], amount: int, max_distance: int = 2
+    ) -> list[tuple[int, int]]:
+        if not self.is_valid_position(central_position):
+            raise ValueError("Central position is out of the matrix")
+
+        max_distance_range = (max_distance * 2 + 1) ** 2
+
+        if amount > max_distance_range:
             raise ValueError(
-                "There are more or less initial positions than drones,"
-                "please make sure there are the same number of initial possitions "
-                "and number of drones."
+                "There are more persons than grid spots. Reduce number of persons or increase grid size."
             )
-        for i in range(len(drones_positions)):
-            x, y = drones_positions[i]
-            self.agents_positions[self.possible_agents[i]] = (x, y)
+
+        unique_random_positions = {central_position}
+        while len(unique_random_positions) < amount:
+            dx = randint(-max_distance, max_distance)
+            dy = randint(-max_distance, max_distance)
+
+            # Checking to avoid including the central position or duplicate positions.
+            if (dx, dy) != (0, 0):
+                new_position = (central_position[0] + dx, central_position[1] + dy)
+                if self.is_valid_position(new_position):
+                    unique_random_positions.add(new_position)
+
+        return list(unique_random_positions)
 
     def render(self):
         self.pygame_renderer.render_map()
-        self.pygame_renderer.render_drones(self.agents_positions.values())
-        self.pygame_renderer.render_person(self.person_x, self.person_y)
+        self.pygame_renderer.render_entities(self.persons_set)
+        self.pygame_renderer.render_entities(self.agents_positions)
         self.pygame_renderer.refresh_screen()
 
-
     def reset(
-            self,
-            seed=None,
-            return_info=False,
-            options=None,
-            drones_positions=None,
-            vector=None,
+        self,
+        seed=None,
+        options=None,
     ):
-        self._was_reset = True
-        
-        if drones_positions is not None:
-            if not self.is_valid_position_drones(drones_positions):
-                raise ValueError("You are trying to place the drone in a invalid position")
-
-        # reset target position
-        self.person_y = self.person_initial_position[1]
-        self.person_x = self.person_initial_position[0]
-
-        self.agents = copy(self.possible_agents)
-        self.timestep = 0
-        self.vector = vector if vector else self.vector
+        self.persons_set = self.create_persons_set()
+        for person in self.persons_set:
+            person.reset_position()
+            person.update_time_step_relation(self.time_step_relation, self.cell_size)
+
+        pod_multiplier = options.get("person_pod_multipliers") if options else None
+
+        if pod_multiplier is not None:
+            self.raise_if_unvalid_mult(pod_multiplier)
+            for person, mult in zip(self.persons_set, pod_multiplier):
+                person.set_mult(mult)
+
+        observations, infos = super().reset(seed=seed, options=options)
         self.rewards_sum = {a: 0 for a in self.agents}
         self.rewards_sum["total"] = 0
-        self.probability_matrix = ProbabilityMatrix(
-            40,
-            self.disperse_constant,
-            self.disperse_constant,
-            self.vector,
-            [self.person_initial_position[1], self.person_initial_position[0]],
-            self.grid_size,
-        )
-        
-        if drones_positions is None:
-            self.default_drones_positions()
-        else:
-            self.required_drone_positions(drones_positions)
-        
-        if self.render_mode == "human":
-            self.pygame_renderer.probability_matrix = self.probability_matrix
-            self.pygame_renderer.enable_render()
-            self.render()
+        return observations, infos
 
-        observations = self.create_observations()
-        return observations
-    
-    def is_valid_position_drones(self, positions: list[tuple[int, int]]) -> bool:
-        seen = set()
-        for position in positions:
-            if not self.is_valid_position(position) or position in seen:
-                return False
-            seen.add(position)
-        return True
+    def raise_if_unvalid_mult(self, individual_multiplication: list[int]) -> bool:
+        if len(individual_multiplication) != len(self.persons_set):
+            raise ValueError(
+                "The number of multipliers must be equal to the number of persons."
+            )
+
+        for mult in individual_multiplication:
+            if not isinstance(mult, (int, float)) or mult < 0:
+                raise ValueError("The multiplier must be a positive number.")
+
+    def pre_search_simulate(self):
+        for _ in range(self.pre_render_steps):
+            self.create_observations()
+            if self.render_mode == "human":
+                self.render()
 
-    
     def create_observations(self):
         observations = {}
-        self.probability_matrix.step()
 
-        movement_map = self.build_movement_matrix()
+        for person in self.persons_set:
+            movement_map = self.build_movement_matrix(person)
+            person.step(movement_map)
 
-        movement = update_shipwrecked_position(movement_map)
-        actual_movement = noise_person_movement(movement, self.vector, epsilon=0.0)
-        
-        self.person_x = self.safe_1d_position_update(self.person_x, actual_movement[0])
-        self.person_y = self.safe_1d_position_update(self.person_y, actual_movement[1])
+        self.probability_matrix.step()
 
         probability_matrix = self.probability_matrix.get_matrix()
-        for agent in self.possible_agents:
+        for idx, agent in enumerate(self.agents):
             observation = (
-                (self.agents_positions[agent][0], self.agents_positions[agent][1]),
+                self.agents_positions[idx],
                 probability_matrix,
             )
-            observations[agent] = {"observation": observation}
+            observations[agent] = observation
 
         return observations
 
-    def build_movement_matrix(self) -> np.array:
-        """
-        Builds and outputs a 3x3 matrix from the probabality matrix to use in the person movement function.
-        """
-        
-        # Boundaries for the 3x3 movement matrix.
-        left_x = max(self.person_x - 1, 0)
-        right_x = min(self.person_x + 2, self.grid_size)
-        left_y = max(self.person_y - 1, 0)
-        right_y = min(self.person_y + 2, self.grid_size)
-
-        probability_matrix = self.probability_matrix.get_matrix()
-        movement_map = probability_matrix[left_y:right_y, left_x:right_x]
-
-        # Pad the matrix
-        if self.person_x == 0:
-            movement_map = np.insert(movement_map, 0, 0, axis=1)
-        elif self.person_x == self.grid_size - 1:
-            movement_map = np.insert(movement_map, 2, 0, axis=1)
-        
-        if self.person_y == 0:
-            movement_map = np.insert(movement_map, 0, 0, axis=0)
-        elif self.person_y == self.grid_size - 1:
-            movement_map = np.insert(movement_map, 2, 0, axis=0)
-        
-        return movement_map
-
-
-
-    def safe_1d_position_update(self, previous: int, movement: int) -> int:
-        """
-        Updates the shipwrecked person position on a given axis, checking for edge cases first.
-
-        Output:
-            new position: int
-        """
-        new_position_on_axis = previous + movement
-        if new_position_on_axis >= 0 and new_position_on_axis < self.grid_size:
-            return new_position_on_axis
-        return previous
- 
-
-    def move_drone(self, position, action):
-        """
-        Returns a tuple with (is_terminal, new_position, reward)
-        """
-        match action:
-            case Actions.LEFT.value:  # LEFT
-                new_position = (position[0] - 1, position[1])
-            case Actions.RIGHT.value:  # RIGHT
-                new_position = (position[0] + 1, position[1])
-            case Actions.UP.value:  # UP
-                new_position = (position[0], position[1] - 1)
-            case Actions.DOWN.value:  # DOWN
-                new_position = (position[0], position[1] + 1)
-            case Actions.UP_LEFT.value:  # UP_LEFT
-                new_position = (position[0] - 1, position[1] - 1)
-            case Actions.UP_RIGHT.value:  # UP_RIGHT
-                new_position = (position[0] + 1, position[1] - 1)
-            case Actions.DOWN_LEFT.value:  # DOWN_LEFT
-                new_position = (position[0] - 1, position[1] + 1)
-            case Actions.DOWN_RIGHT.value:  # DOWN_RIGHT
-                new_position = (position[0] + 1, position[1] + 1)
-
-        if not self.is_valid_position(new_position):
-            return True, new_position, self.reward_scheme["leave_grid"]
-
-        return False, new_position, self.reward_scheme["default"]
-
     def step(self, actions):
         """
         Returns a tuple with (observations, rewards, terminations, truncations, infos)
         """
         if not self._was_reset:
             raise ValueError("Please reset the env before interacting with it")
-        
+
         terminations = {a: False for a in self.agents}
-        rewards = {a: self.reward_scheme["default"] for a in self.agents}
+        rewards = {a: self.reward_scheme.default for a in self.agents}
         truncations = {a: False for a in self.agents}
         person_found = False
-        
-        for agent in self.agents:
+
+        for idx, agent in enumerate(self.agents):
             if agent not in actions:
                 raise ValueError("Missing action for " + agent)
 
             drone_action = actions[agent]
             if drone_action not in self.action_space(agent):
                 raise ValueError("Invalid action for " + agent)
 
-            drone_x = self.agents_positions[agent][0]
-            drone_y = self.agents_positions[agent][1]
+            # Check truncation conditions (overwrites termination conditions)
+            if self.timestep >= self.timestep_limit:
+                # TODO: Check if is really necessary to add rewards_sum into this reward
+                rewards[agent] = self.reward_scheme.exceed_timestep
+                if self.rewards_sum[agent] > 0:
+                    rewards[agent] += self.rewards_sum[agent] // 2
+                truncations[agent] = True
+                terminations[agent] = True
+                continue
+
+            drone_x, drone_y = self.agents_positions[idx]
             is_searching = drone_action == Actions.SEARCH.value
 
             if drone_action != Actions.SEARCH.value:
-                is_terminal, new_position, reward = self.move_drone(
-                    (drone_x, drone_y), drone_action
+                new_position = self.move_drone((drone_x, drone_y), drone_action)
+                if not self.is_valid_position(new_position):
+                    rewards[agent] = self.reward_scheme.leave_grid
+                else:
+                    self.agents_positions[idx] = new_position
+                    rewards[agent] = self.reward_scheme.default
+                self.rewards_sum[agent] += rewards[agent]
+                continue
+
+            drone_found_person = False
+            for human in self.persons_set:
+                drone_found_person = (
+                    human.x == drone_x and human.y == drone_y and is_searching
                 )
-                self.agents_positions[agent] = new_position
-                rewards[agent] = reward
-                terminations[agent] = is_terminal
-                truncations[agent] = is_terminal
-            
-            drone_found_person = drone_x == self.person_x and drone_y == self.person_y and is_searching
+                if drone_found_person:
+                    break
+
             random_value = random()
-            if drone_found_person and random_value < self.pod:
-                time_reward_corrected = self.reward_scheme["search_and_find"] * (1 - self.timestep / self.timestep_limit)
-                rewards[agent] = self.reward_scheme["search_and_find"] + time_reward_corrected
-                terminations = {a: True for a in self.agents}
-                truncations = {a: True for a in self.agents}
-                person_found = True
+            if drone_found_person:
+                max_detection_probability = min(human.get_mult() * self.drone.pod, 1)
+
+                if random_value <= max_detection_probability:
+                    self.persons_set.remove(human)
+
+                    time_decay_factor = 1 - (self.timestep / self.timestep_limit)
+                    time_reward_corrected = (
+                        self.reward_scheme.search_and_find * time_decay_factor
+                    )
+                    rewards[agent] = (
+                        self.reward_scheme.search_and_find + time_reward_corrected
+                    )
+
+                if len(self.persons_set) == 0:
+                    person_found = True
+                    for agent in self.agents:
+                        terminations[agent] = True
+                        truncations[agent] = True
             elif is_searching:
                 prob_matrix = self.probability_matrix.get_matrix()
-                rewards[agent] = prob_matrix[drone_y][drone_x] * 10000 if prob_matrix[drone_y][drone_x] * 100 > 1 else -100
-
-            # Check truncation conditions (overwrites termination conditions)
-            # TODO: Think, should this be >= ??
-            if self.timestep > self.timestep_limit:
-                rewards[agent] = self.rewards_sum[agent] * -1 + self.reward_scheme["exceed_timestep"]
-                truncations[agent] = True
-                terminations[agent] = True
+                rewards[agent] = (
+                    prob_matrix[drone_y][drone_x] * 10000
+                    if prob_matrix[drone_y][drone_x] * 100 > 1
+                    else -100
+                )
 
             self.rewards_sum[agent] += rewards[agent]
 
         self.timestep += 1
-        # Get observations
-        observations = self.create_observations()
         # Get dummy infos
-        infos = {"Found": person_found}
+        infos = {drone: {"Found": person_found} for drone in self.agents}
 
         # CHECK COLISION - Drone
-        self.compute_drone_collision(terminations, rewards, truncations)
-        rewards["total_reward"] = sum(rewards.values())
-        self.rewards_sum["total"] += rewards["total_reward"]
+        self.compute_drone_collision(terminations, rewards)
+        # TODO: Check real usage of this, gives error when using w/ RL libs
+        # rewards["total_reward"] = sum(rewards.values())
+        # self.rewards_sum["total"] += rewards["total_reward"]
 
-        self.render_step(any(terminations.values()), person_found)        
+        self.render_step(any(terminations.values()), person_found)
 
+        # Get observations
+        observations = self.create_observations()
+        # If terminated, reset the agents (pettingzoo parallel env requirement)
+        if any(terminations.values()) or any(truncations.values()):
+            self.agents = []
         return observations, rewards, terminations, truncations, infos
-    
-    def compute_drone_collision(self, terminations, rewards, truncations):
-        """
-        Check for drone collision and compute terminations, rewards and truncations.
-        """
-        
-        for drone_1_id, drone_1_position in self.agents_positions.items():
-            for drone_2_id, drone_2_position in self.agents_positions.items():
-                if drone_1_id == drone_2_id:
-                    continue
-            
-                if drone_1_position[0] == drone_2_position[0] and drone_1_position[1] == drone_2_position[1]:
-                    truncations[drone_1_id] = True
-                    terminations[drone_1_id] = True
-                    rewards[drone_1_id] = self.reward_scheme["drones_collision"]
-
 
     def render_step(self, terminal, person_found):
         if self.render_mode == "human":
             if terminal:
                 if person_found:
-                    self.pygame_renderer.render_episode_end_screen(f"The target was found in {self.timestep} moves", GREEN)
+                    self.pygame_renderer.render_episode_end_screen(
+                        f"The target was found in {self.timestep} moves", GREEN
+                    )
                 else:
-                    self.pygame_renderer.render_episode_end_screen("The target was not found.", RED)
+                    self.pygame_renderer.render_episode_end_screen(
+                        "The target was not found.", RED
+                    )
             else:
                 self.render()
 
+    def build_movement_matrix(self, person: Person) -> np.ndarray:
+        """
+        Builds and outputs a 3x3 matrix from the probabality matrix to use in the person movement function.
+        """
+        # Boundaries for the 3x3 movement matrix.
+        left_x = max(person.x - 1, 0)
+        right_x = min(person.x + 2, self.grid_size)
+        left_y = max(person.y - 1, 0)
+        right_y = min(person.y + 2, self.grid_size)
+
+        probability_matrix = self.probability_matrix.get_matrix()
+        movement_map = probability_matrix[left_y:right_y, left_x:right_x].copy()
+
+        # Pad the matrix
+        if person.x == 0:
+            movement_map = np.insert(movement_map, 0, 0, axis=1)
+        elif person.x == self.grid_size - 1:
+            movement_map = np.insert(movement_map, 2, 0, axis=1)
+
+        if person.y == 0:
+            movement_map = np.insert(movement_map, 0, 0, axis=0)
+        elif person.y == self.grid_size - 1:
+            movement_map = np.insert(movement_map, 2, 0, axis=0)
+
+        return movement_map
 
-    def get_agents(self):
-        return self.possible_agents
+    def get_persons(self):
+        return self.persons_set
 
     @functools.lru_cache(maxsize=None)
     def observation_space(self, agent):
-        # TODO: If x and y are the observation, then this should the observation space
-        return MultiDiscrete([self.grid_size] * 2)
+        # Observation space for each agent:
+        # - MultiDiscrete: (x, y) position of the agent
+        # - Box: Probability matrix
+        return Tuple(
+            (
+                MultiDiscrete([self.grid_size, self.grid_size]),
+                Box(
+                    low=0,
+                    high=1,
+                    shape=(self.grid_size, self.grid_size),
+                    dtype=np.float32,
+                ),
+            )
+        )
 
     @functools.lru_cache(maxsize=None)
     def action_space(self, agent):
-        return [moviment.value for moviment in Actions]
+        return Discrete(len(self.possible_actions))
```

### Comparing `DSSE-0.2.4/DSSE/environment/imgs/drone.png` & `dsse-1.0.0/DSSE/environment/imgs/drone.png`

 * *Files identical despite different names*

### Comparing `DSSE-0.2.4/DSSE/environment/imgs/person-swimming.png` & `dsse-1.0.0/DSSE/environment/imgs/person-swimming.png`

 * *Files identical despite different names*

### Comparing `DSSE-0.2.4/DSSE/environment/pygame_interface.py` & `dsse-1.0.0/DSSE/environment/pygame_interface.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,75 +6,85 @@
 
 
 class PygameInterface:
     """
     Class for rendering the grafical interface of the simulation
     """
 
-    FPS = 3
+    FPS = 5
 
     def __init__(
         self, grid_size: int, render_gradient: bool, render_grid: bool
     ) -> None:
         pygame.init()
         self.grid_size = grid_size
         self.render_gradient = render_gradient
         self.render_grid = render_grid
         self.window_size = 700
-        self.screen = pygame.Surface([self.window_size + 20, self.window_size + 20])
+        self.screen = None
         self.render_on = False
         self.probability_matrix = None
 
         self.block_size = self.window_size / self.grid_size
         self.drone_img = None
         self.person_img = None
         self.clock = None
 
     def render_map(self):
         self.draw()
 
         for event in pygame.event.get():
             if event.type == pygame.QUIT:
                 self.close()
+
         pygame.event.pump()
 
     def refresh_screen(self):
         pygame.display.flip()
 
     def enable_render(self):
         if self.render_on:
             return
 
+        self.screen = pygame.Surface([self.window_size + 20, self.window_size + 20])
         self.screen = pygame.display.set_mode(self.screen.get_size())
 
         current_directory = os.path.dirname(os.path.abspath(__file__))
-        self.drone_img = self.load_and_scale_image(f"{current_directory}/imgs/drone.png")
-        self.person_img = self.load_and_scale_image(f"{current_directory}/imgs/person-swimming.png")
+        self.drone_img = self.load_and_scale_image(
+            f"{current_directory}/imgs/drone.png"
+        )
+        self.person_img = self.load_and_scale_image(
+            f"{current_directory}/imgs/person-swimming.png"
+        )
 
         self.clock = pygame.time.Clock()
         self.render_on = True
 
     def load_and_scale_image(self, image_path: str):
         loaded_img = pygame.image.load(image_path).convert()
         scaled_img = pygame.transform.scale(
             loaded_img, (self.block_size, self.block_size)
         )
         return scaled_img
 
-    def render_drones(self, drone_positions) -> None:
-        for position in drone_positions:
-            rectangle = self.get_position_rectangle(position)
-            self.screen.blit(self.drone_img, rectangle)
-
-    def render_person(self, person_x: int, person_y: int) -> None:
-        self.screen.blit(
-            self.person_img, self.get_position_rectangle((person_x, person_y))
-        )
+    def render_entities(self, entities) -> None:
+        for entity in entities:
+            # Checks if the entity is a tuple (assuming that drones are represented as tuples).
+            if isinstance(entity, tuple):
+                rectangle = self.get_position_rectangle(entity)
+                image = self.drone_img
+            # Otherwise, assumes it is an object with 'x' and 'y' attributes (such as a person).
+            else:
+                rectangle = self.get_position_rectangle((entity.x, entity.y))
+                image = self.person_img
+
+            # Renders the entity.
+            self.screen.blit(image, rectangle)
 
-    def get_position_rectangle(self, position: tuple[int]) -> pygame.Rect:
+    def get_position_rectangle(self, position: tuple[int, int]) -> pygame.Rect:
         x = 10 + self.block_size * position[0]
         y = 10 + self.block_size * position[1]
         return pygame.Rect(x, y, self.block_size, self.block_size)
 
     def draw(self):
         self.clock.tick(self.FPS)
         self.screen.fill(BLACK)
```

### Comparing `DSSE-0.2.4/DSSE.egg-info/PKG-INFO` & `dsse-1.0.0/DSSE.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,46 +1,47 @@
 Metadata-Version: 2.1
 Name: DSSE
-Version: 0.2.4
+Version: 1.0.0
 Summary: An environment to train drones to search and find a shipwrecked person lost in the ocean using reinforcement learning.
 Home-page: https://github.com/pfeinsper/drone-swarm-search
-Author: Luis Filipe Carrete, Manuel Castanares, Enrico Damiani, Leonardo Malta, Joras Oliveira, Ricardo Ribeiro Rodrigues, Renato Lafrachi Falcao, Pedro Andrade, Fabricio Barth
+Download-URL: https://github.com/pfeinsper/drone-swarm-search/archive/refs/tags/v1.0.0.tar.gz
+Author: Luis Filipe Carrete, Manuel Castanares, Enrico Damiani, Leonardo Malta, Jorás Oliveira, Ricardo Ribeiro Rodrigues, Renato Laffranchi Falcão, Pedro Henrique Britto Aragão Andrade, Fabricio Barth
 License: MIT
-Download-URL: https://github.com/pfeinsper/drone-swarm-search/archive/refs/tags/v0.2.2.tar.gz
 Keywords: Reinforcement Learning,AI,SAR,Multi Agent
-Platform: UNKNOWN
 Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: numpy
+Requires-Dist: gymnasium
+Requires-Dist: pygame
+Requires-Dist: pettingzoo
+Requires-Dist: matplotlib
+Requires-Dist: numba
+
+[![Tests Status 🧪](https://github.com/pfeinsper/drone-swarm-search/actions/workflows/env.yml/badge.svg)](https://github.com/pfeinsper/drone-swarm-search/actions/workflows/env.yml) [![Docs Deployment 📝](https://github.com/pfeinsper/drone-swarm-search/actions/workflows/deploy.yml/badge.svg?branch=vitepress_docs)](https://github.com/pfeinsper/drone-swarm-search/actions/workflows/deploy.yml) [![PyPI Release 🚀](https://badge.fury.io/py/DSSE.svg)](https://badge.fury.io/py/DSSE) [![License: MIT](https://img.shields.io/badge/License-MIT-brightgreen.svg?style=flat)](https://github.com/pfeinsper/drone-swarm-search/blob/main/LICENSE)
 
 # Drone Swarm Search
 
-## Workflow Status: Automated Testing with Pytest
+The Drone Swarm Search project is an environment, based on PettingZoo, that is to be used in conjunction with multi-agent (or single-agent) reinforcement learning algorithms. It is an environment in which the agents (drones), have to find the targets (shipwrecked people). The agents do not know the position of the target, and do not receive rewards related to their own distance to the target(s). However, the agents receive the probabilities of the target(s) being in a certain cell of the map. The aim of this project is to aid in the study of reinforcement learning algorithms that require dynamic probabilities as inputs. A visual representation of the environment is displayed below. To test the environment (without an algorithm), run `basic_env.py`.
 
-[![Run Pytest](https://github.com/pfeinsper/drone-swarm-search/actions/workflows/env.yml/badge.svg)](https://github.com/pfeinsper/drone-swarm-search/actions/workflows/env.yml)
+<p align="center">
+    <img src="https://raw.github.com/PFE-Embraer/drone-swarm-search/env-cleanup/docs/gifs/render_with_grid_gradient.gif" width="400" height="400" align="center">
+</p>
 
 ## Quick Start
 
 #### Install
 `pip install DSSE`
 
 #### Use
 `from DSSE.env import DroneSwarmSearch`
 
 #### PyPi Package Page
 
 https://pypi.org/project/DSSE/
 
-## About
-
-The Drone Swarm Search project is an environment, based on PettingZoo, that is to be used in conjunction with multi-agent (or single-agent) reinforcement learning algorithms. It is an environment in which the agents (drones), have to find the targets (shipwrecked people). The agents do not know the position of the target, and do not receive rewards related to their own distance to the target(s). However, the agents receive the probabilities of the target(s) being in a certain cell of the map. The aim of this project is to aid in the study of reinforcement learning algorithms that require dynamic probabilities as inputs. A visual representation of the environment is displayed below. To test the environment (without an algorithm), run `basic_env.py`.
-
-<p align="center">
-    <img src="https://raw.github.com/PFE-Embraer/drone-swarm-search/env-cleanup/docs/gifs/render_with_grid_gradient.gif" width="400" height="400" align="center">
-</p>
-
-
 ## Outcome
 
 | If drone is found            | If drone is not found  |
 :-------------------------:|:-------------------------:
 | ![](https://raw.githubusercontent.com/PFE-Embraer/drone-swarm-search/main/docs/pics/victory_render.png)     | ![](https://raw.github.com/PFE-Embraer/drone-swarm-search/main/docs/pics/fail_render.png) |
 
 
@@ -281,9 +282,7 @@
       year={2023},
       eprint={2307.06240},
       archivePrefix={arXiv},
       primaryClass={cs.LG},
       doi={https://doi.org/10.48550/arXiv.2307.06240}
 }
 ```
-
-
```

### Comparing `DSSE-0.2.4/PKG-INFO` & `dsse-1.0.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,46 +1,47 @@
 Metadata-Version: 2.1
 Name: DSSE
-Version: 0.2.4
+Version: 1.0.0
 Summary: An environment to train drones to search and find a shipwrecked person lost in the ocean using reinforcement learning.
 Home-page: https://github.com/pfeinsper/drone-swarm-search
-Author: Luis Filipe Carrete, Manuel Castanares, Enrico Damiani, Leonardo Malta, Joras Oliveira, Ricardo Ribeiro Rodrigues, Renato Lafrachi Falcao, Pedro Andrade, Fabricio Barth
+Download-URL: https://github.com/pfeinsper/drone-swarm-search/archive/refs/tags/v1.0.0.tar.gz
+Author: Luis Filipe Carrete, Manuel Castanares, Enrico Damiani, Leonardo Malta, Jorás Oliveira, Ricardo Ribeiro Rodrigues, Renato Laffranchi Falcão, Pedro Henrique Britto Aragão Andrade, Fabricio Barth
 License: MIT
-Download-URL: https://github.com/pfeinsper/drone-swarm-search/archive/refs/tags/v0.2.2.tar.gz
 Keywords: Reinforcement Learning,AI,SAR,Multi Agent
-Platform: UNKNOWN
 Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: numpy
+Requires-Dist: gymnasium
+Requires-Dist: pygame
+Requires-Dist: pettingzoo
+Requires-Dist: matplotlib
+Requires-Dist: numba
+
+[![Tests Status 🧪](https://github.com/pfeinsper/drone-swarm-search/actions/workflows/env.yml/badge.svg)](https://github.com/pfeinsper/drone-swarm-search/actions/workflows/env.yml) [![Docs Deployment 📝](https://github.com/pfeinsper/drone-swarm-search/actions/workflows/deploy.yml/badge.svg?branch=vitepress_docs)](https://github.com/pfeinsper/drone-swarm-search/actions/workflows/deploy.yml) [![PyPI Release 🚀](https://badge.fury.io/py/DSSE.svg)](https://badge.fury.io/py/DSSE) [![License: MIT](https://img.shields.io/badge/License-MIT-brightgreen.svg?style=flat)](https://github.com/pfeinsper/drone-swarm-search/blob/main/LICENSE)
 
 # Drone Swarm Search
 
-## Workflow Status: Automated Testing with Pytest
+The Drone Swarm Search project is an environment, based on PettingZoo, that is to be used in conjunction with multi-agent (or single-agent) reinforcement learning algorithms. It is an environment in which the agents (drones), have to find the targets (shipwrecked people). The agents do not know the position of the target, and do not receive rewards related to their own distance to the target(s). However, the agents receive the probabilities of the target(s) being in a certain cell of the map. The aim of this project is to aid in the study of reinforcement learning algorithms that require dynamic probabilities as inputs. A visual representation of the environment is displayed below. To test the environment (without an algorithm), run `basic_env.py`.
 
-[![Run Pytest](https://github.com/pfeinsper/drone-swarm-search/actions/workflows/env.yml/badge.svg)](https://github.com/pfeinsper/drone-swarm-search/actions/workflows/env.yml)
+<p align="center">
+    <img src="https://raw.github.com/PFE-Embraer/drone-swarm-search/env-cleanup/docs/gifs/render_with_grid_gradient.gif" width="400" height="400" align="center">
+</p>
 
 ## Quick Start
 
 #### Install
 `pip install DSSE`
 
 #### Use
 `from DSSE.env import DroneSwarmSearch`
 
 #### PyPi Package Page
 
 https://pypi.org/project/DSSE/
 
-## About
-
-The Drone Swarm Search project is an environment, based on PettingZoo, that is to be used in conjunction with multi-agent (or single-agent) reinforcement learning algorithms. It is an environment in which the agents (drones), have to find the targets (shipwrecked people). The agents do not know the position of the target, and do not receive rewards related to their own distance to the target(s). However, the agents receive the probabilities of the target(s) being in a certain cell of the map. The aim of this project is to aid in the study of reinforcement learning algorithms that require dynamic probabilities as inputs. A visual representation of the environment is displayed below. To test the environment (without an algorithm), run `basic_env.py`.
-
-<p align="center">
-    <img src="https://raw.github.com/PFE-Embraer/drone-swarm-search/env-cleanup/docs/gifs/render_with_grid_gradient.gif" width="400" height="400" align="center">
-</p>
-
-
 ## Outcome
 
 | If drone is found            | If drone is not found  |
 :-------------------------:|:-------------------------:
 | ![](https://raw.githubusercontent.com/PFE-Embraer/drone-swarm-search/main/docs/pics/victory_render.png)     | ![](https://raw.github.com/PFE-Embraer/drone-swarm-search/main/docs/pics/fail_render.png) |
 
 
@@ -281,9 +282,7 @@
       year={2023},
       eprint={2307.06240},
       archivePrefix={arXiv},
       primaryClass={cs.LG},
       doi={https://doi.org/10.48550/arXiv.2307.06240}
 }
 ```
-
-
```

### Comparing `DSSE-0.2.4/README.md` & `dsse-1.0.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,34 +1,29 @@
+[![Tests Status 🧪](https://github.com/pfeinsper/drone-swarm-search/actions/workflows/env.yml/badge.svg)](https://github.com/pfeinsper/drone-swarm-search/actions/workflows/env.yml) [![Docs Deployment 📝](https://github.com/pfeinsper/drone-swarm-search/actions/workflows/deploy.yml/badge.svg?branch=vitepress_docs)](https://github.com/pfeinsper/drone-swarm-search/actions/workflows/deploy.yml) [![PyPI Release 🚀](https://badge.fury.io/py/DSSE.svg)](https://badge.fury.io/py/DSSE) [![License: MIT](https://img.shields.io/badge/License-MIT-brightgreen.svg?style=flat)](https://github.com/pfeinsper/drone-swarm-search/blob/main/LICENSE)
+
 # Drone Swarm Search
 
-## Workflow Status: Automated Testing with Pytest
+The Drone Swarm Search project is an environment, based on PettingZoo, that is to be used in conjunction with multi-agent (or single-agent) reinforcement learning algorithms. It is an environment in which the agents (drones), have to find the targets (shipwrecked people). The agents do not know the position of the target, and do not receive rewards related to their own distance to the target(s). However, the agents receive the probabilities of the target(s) being in a certain cell of the map. The aim of this project is to aid in the study of reinforcement learning algorithms that require dynamic probabilities as inputs. A visual representation of the environment is displayed below. To test the environment (without an algorithm), run `basic_env.py`.
 
-[![Run Pytest](https://github.com/pfeinsper/drone-swarm-search/actions/workflows/env.yml/badge.svg)](https://github.com/pfeinsper/drone-swarm-search/actions/workflows/env.yml)
+<p align="center">
+    <img src="https://raw.github.com/PFE-Embraer/drone-swarm-search/env-cleanup/docs/gifs/render_with_grid_gradient.gif" width="400" height="400" align="center">
+</p>
 
 ## Quick Start
 
 #### Install
 `pip install DSSE`
 
 #### Use
 `from DSSE.env import DroneSwarmSearch`
 
 #### PyPi Package Page
 
 https://pypi.org/project/DSSE/
 
-## About
-
-The Drone Swarm Search project is an environment, based on PettingZoo, that is to be used in conjunction with multi-agent (or single-agent) reinforcement learning algorithms. It is an environment in which the agents (drones), have to find the targets (shipwrecked people). The agents do not know the position of the target, and do not receive rewards related to their own distance to the target(s). However, the agents receive the probabilities of the target(s) being in a certain cell of the map. The aim of this project is to aid in the study of reinforcement learning algorithms that require dynamic probabilities as inputs. A visual representation of the environment is displayed below. To test the environment (without an algorithm), run `basic_env.py`.
-
-<p align="center">
-    <img src="https://raw.github.com/PFE-Embraer/drone-swarm-search/env-cleanup/docs/gifs/render_with_grid_gradient.gif" width="400" height="400" align="center">
-</p>
-
-
 ## Outcome
 
 | If drone is found            | If drone is not found  |
 :-------------------------:|:-------------------------:
 | ![](https://raw.githubusercontent.com/PFE-Embraer/drone-swarm-search/main/docs/pics/victory_render.png)     | ![](https://raw.github.com/PFE-Embraer/drone-swarm-search/main/docs/pics/fail_render.png) |
```

### Comparing `DSSE-0.2.4/setup.py` & `dsse-1.0.0/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,33 +1,28 @@
-from setuptools import setup
+from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding="utf-8") as f:
     long_description = f.read()
 
 
 download_url = (
-    "https://github.com/pfeinsper/drone-swarm-search/archive/refs/tags/v0.2.2.tar.gz"
+    f"https://github.com/pfeinsper/drone-swarm-search/archive/refs/tags/v1.0.0.tar.gz"
 )
 setup(
     name="DSSE",
-    version="0.2.4",
-    author="Luis Filipe Carrete, Manuel Castanares, Enrico Damiani, Leonardo Malta, Joras Oliveira, Ricardo Ribeiro Rodrigues, Renato Lafrachi Falcao, Pedro Andrade, Fabricio Barth",
+    version="1.0.0",
+    author="Luis Filipe Carrete, Manuel Castanares, Enrico Damiani, Leonardo Malta, Jorás Oliveira, Ricardo Ribeiro Rodrigues, Renato Laffranchi Falcão, Pedro Henrique Britto Aragão Andrade, Fabricio Barth",
     description="An environment to train drones to search and find a shipwrecked person lost in the ocean using reinforcement learning.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/pfeinsper/drone-swarm-search",
     license="MIT",
     keywords=["Reinforcement Learning", "AI", "SAR", "Multi Agent"],
     download_url=download_url,
-    packages=[
-        "DSSE",
-        "DSSE.environment",
-        "DSSE.environment.imgs",
-        "DSSE.environment.generator",
-    ],
+    packages=find_packages(),
     include_package_data=True,
     package_data={"DSSE": ["environment/imgs/*.png"]},
     install_requires=[
         "numpy",
         "gymnasium",
         "pygame",
         "pettingzoo",
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

