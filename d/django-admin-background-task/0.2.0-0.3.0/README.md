# Comparing `tmp/django_admin_background_task-0.2.0.tar.gz` & `tmp/django_admin_background_task-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_admin_background_task-0.2.0.tar", max compression
+gzip compressed data, was "django_admin_background_task-0.3.0.tar", max compression
```

## Comparing `django_admin_background_task-0.2.0.tar` & `django_admin_background_task-0.3.0.tar`

### file list

```diff
@@ -1,28 +1,29 @@
--rw-r--r--   0        0        0    11357 2024-03-08 11:29:40.116270 django_admin_background_task-0.2.0/LICENSE
--rw-r--r--   0        0        0      597 2024-03-08 15:24:11.483284 django_admin_background_task-0.2.0/README.md
--rw-r--r--   0        0        0        0 2024-03-08 11:30:13.723481 django_admin_background_task-0.2.0/bgtask/__init__.py
--rw-r--r--   0        0        0      965 2024-04-16 15:31:09.755506 django_admin_background_task-0.2.0/bgtask/admin.py
--rw-r--r--   0        0        0      144 2024-03-08 11:30:13.729684 django_admin_background_task-0.2.0/bgtask/apps.py
--rw-r--r--   0        0        0       57 2024-03-10 23:21:32.768101 django_admin_background_task-0.2.0/bgtask/backends/__init__.py
--rw-r--r--   0        0        0      304 2024-03-10 23:20:51.665708 django_admin_background_task-0.2.0/bgtask/backends/thread_pool.py
--rw-r--r--   0        0        0     1119 2024-04-16 15:15:56.816234 django_admin_background_task-0.2.0/bgtask/decorators.py
--rw-r--r--   0        0        0     2013 2024-03-08 11:30:13.719326 django_admin_background_task-0.2.0/bgtask/migrations/0001_initial.py
--rw-r--r--   0        0        0      968 2024-04-16 14:59:49.149350 django_admin_background_task-0.2.0/bgtask/migrations/0002_backgroundtask_namespace_alter_backgroundtask_name.py
--rw-r--r--   0        0        0        0 2024-03-08 11:30:13.714396 django_admin_background_task-0.2.0/bgtask/migrations/__init__.py
--rw-r--r--   0        0        0     2925 2024-04-16 15:13:30.710650 django_admin_background_task-0.2.0/bgtask/model_admin.py
--rw-r--r--   0        0        0     9184 2024-04-16 15:32:37.932296 django_admin_background_task-0.2.0/bgtask/models.py
--rw-r--r--   0        0        0      231 2024-03-08 11:30:13.721685 django_admin_background_task-0.2.0/bgtask/stack_contexts.py
--rw-r--r--   0        0        0      746 2024-03-08 11:30:13.732726 django_admin_background_task-0.2.0/bgtask/static/bgtask/js/bgtask-once.js
--rw-r--r--   0        0        0    13151 2024-03-12 15:54:33.635207 django_admin_background_task-0.2.0/bgtask/static/bgtask/js/bgtask.js
--rw-r--r--   0        0        0     1062 2024-04-14 14:54:44.154777 django_admin_background_task-0.2.0/bgtask/templates/bgtask/admin/change_list.html
--rw-r--r--   0        0        0      978 2024-03-12 15:14:21.911729 django_admin_background_task-0.2.0/bgtask/templates/bgtask/bg_changelist_status_column.html
--rw-r--r--   0        0        0        1 2024-03-08 11:30:13.737691 django_admin_background_task-0.2.0/bgtask/templates/bgtask/bgtask_templates.html
--rw-r--r--   0        0        0     1845 2024-03-08 11:30:13.736549 django_admin_background_task-0.2.0/bgtask/templates/bgtask/bgtask_view.html
--rw-r--r--   0        0        0      166 2024-03-08 11:30:13.735684 django_admin_background_task-0.2.0/bgtask/templates/bgtask/progress.html
--rw-r--r--   0        0        0        0 2024-03-08 11:30:13.710598 django_admin_background_task-0.2.0/bgtask/templatetags/__init__.py
--rw-r--r--   0        0        0      413 2024-03-08 11:30:13.710386 django_admin_background_task-0.2.0/bgtask/templatetags/bgtask.py
--rw-r--r--   0        0        0     1090 2024-03-08 11:30:13.723311 django_admin_background_task-0.2.0/bgtask/tests/test_bgtask.py
--rw-r--r--   0        0        0      161 2024-03-08 11:30:13.738363 django_admin_background_task-0.2.0/bgtask/urls.py
--rw-r--r--   0        0        0     1765 2024-03-12 15:30:59.663003 django_admin_background_task-0.2.0/bgtask/views.py
--rw-r--r--   0        0        0     1706 2024-03-12 15:36:09.621880 django_admin_background_task-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     1416 1970-01-01 00:00:00.000000 django_admin_background_task-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0    11357 2024-03-08 11:29:40.116270 django_admin_background_task-0.3.0/LICENSE
+-rw-r--r--   0        0        0      597 2024-03-08 15:24:11.483284 django_admin_background_task-0.3.0/README.md
+-rw-r--r--   0        0        0        0 2024-03-08 11:30:13.723481 django_admin_background_task-0.3.0/bgtask/__init__.py
+-rw-r--r--   0        0        0      965 2024-04-16 15:31:09.755506 django_admin_background_task-0.3.0/bgtask/admin.py
+-rw-r--r--   0        0        0      144 2024-03-08 11:30:13.729684 django_admin_background_task-0.3.0/bgtask/apps.py
+-rw-r--r--   0        0        0       57 2024-03-10 23:21:32.768101 django_admin_background_task-0.3.0/bgtask/backends/__init__.py
+-rw-r--r--   0        0        0      304 2024-03-10 23:20:51.665708 django_admin_background_task-0.3.0/bgtask/backends/thread_pool.py
+-rw-r--r--   0        0        0     1119 2024-04-16 15:15:56.816234 django_admin_background_task-0.3.0/bgtask/decorators.py
+-rw-r--r--   0        0        0     2013 2024-03-08 11:30:13.719326 django_admin_background_task-0.3.0/bgtask/migrations/0001_initial.py
+-rw-r--r--   0        0        0      968 2024-04-16 14:59:49.149350 django_admin_background_task-0.3.0/bgtask/migrations/0002_backgroundtask_namespace_alter_backgroundtask_name.py
+-rw-r--r--   0        0        0        0 2024-03-08 11:30:13.714396 django_admin_background_task-0.3.0/bgtask/migrations/__init__.py
+-rw-r--r--   0        0        0     4402 2024-04-18 14:20:52.036965 django_admin_background_task-0.3.0/bgtask/model_admin.py
+-rw-r--r--   0        0        0     9184 2024-04-18 15:16:23.546122 django_admin_background_task-0.3.0/bgtask/models.py
+-rw-r--r--   0        0        0      231 2024-03-08 11:30:13.721685 django_admin_background_task-0.3.0/bgtask/stack_contexts.py
+-rw-r--r--   0        0        0      746 2024-03-08 11:30:13.732726 django_admin_background_task-0.3.0/bgtask/static/bgtask/js/bgtask-once.js
+-rw-r--r--   0        0        0    15026 2024-04-18 15:16:24.511343 django_admin_background_task-0.3.0/bgtask/static/bgtask/js/bgtask.js
+-rw-r--r--   0        0        0     1053 2024-04-18 11:36:40.262228 django_admin_background_task-0.3.0/bgtask/templates/bgtask/admin/change_list.html
+-rw-r--r--   0        0        0      844 2024-04-18 15:05:43.258568 django_admin_background_task-0.3.0/bgtask/templates/bgtask/bg_changelist_status_column.html
+-rw-r--r--   0        0        0      788 2024-04-18 11:08:31.614024 django_admin_background_task-0.3.0/bgtask/templates/bgtask/bg_completed_column.html
+-rw-r--r--   0        0        0        1 2024-03-08 11:30:13.737691 django_admin_background_task-0.3.0/bgtask/templates/bgtask/bgtask_templates.html
+-rw-r--r--   0        0        0     1845 2024-03-08 11:30:13.736549 django_admin_background_task-0.3.0/bgtask/templates/bgtask/bgtask_view.html
+-rw-r--r--   0        0        0      166 2024-03-08 11:30:13.735684 django_admin_background_task-0.3.0/bgtask/templates/bgtask/progress.html
+-rw-r--r--   0        0        0        0 2024-03-08 11:30:13.710598 django_admin_background_task-0.3.0/bgtask/templatetags/__init__.py
+-rw-r--r--   0        0        0      413 2024-03-08 11:30:13.710386 django_admin_background_task-0.3.0/bgtask/templatetags/bgtask.py
+-rw-r--r--   0        0        0     1090 2024-03-08 11:30:13.723311 django_admin_background_task-0.3.0/bgtask/tests/test_bgtask.py
+-rw-r--r--   0        0        0      161 2024-03-08 11:30:13.738363 django_admin_background_task-0.3.0/bgtask/urls.py
+-rw-r--r--   0        0        0     1765 2024-04-18 09:56:48.293063 django_admin_background_task-0.3.0/bgtask/views.py
+-rw-r--r--   0        0        0     1706 2024-04-18 15:14:53.319764 django_admin_background_task-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0     1416 1970-01-01 00:00:00.000000 django_admin_background_task-0.3.0/PKG-INFO
```

### Comparing `django_admin_background_task-0.2.0/LICENSE` & `django_admin_background_task-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `django_admin_background_task-0.2.0/README.md` & `django_admin_background_task-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `django_admin_background_task-0.2.0/bgtask/admin.py` & `django_admin_background_task-0.3.0/bgtask/admin.py`

 * *Files identical despite different names*

### Comparing `django_admin_background_task-0.2.0/bgtask/decorators.py` & `django_admin_background_task-0.3.0/bgtask/decorators.py`

 * *Files identical despite different names*

### Comparing `django_admin_background_task-0.2.0/bgtask/migrations/0001_initial.py` & `django_admin_background_task-0.3.0/bgtask/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django_admin_background_task-0.2.0/bgtask/migrations/0002_backgroundtask_namespace_alter_backgroundtask_name.py` & `django_admin_background_task-0.3.0/bgtask/migrations/0002_backgroundtask_namespace_alter_backgroundtask_name.py`

 * *Files identical despite different names*

### Comparing `django_admin_background_task-0.2.0/bgtask/model_admin.py` & `django_admin_background_task-0.3.0/bgtask/model_admin.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,24 +1,47 @@
 from datetime import timedelta
+from functools import wraps
 
 from django.contrib import admin
 from django.contrib.admin.utils import label_for_field
+from django.contrib.messages import INFO
 from django.db.models import Q
 from django.utils import timezone
 
 from .models import BackgroundTask
 
 
 class BGTaskModelAdmin(admin.ModelAdmin):
     # This is not overridden to avoid messing with the implicit logic for finding change list
     # templates that ModelAdmin uses. So you either need to specify this yourself on your
     # subclass or you need to extend from this in your custom template.
+    #
     # change_list_template = "bgtask/admin/change_list.html"
 
     # ----------------------------------------------------------------------------------------------
+    # Class API
+    # ----------------------------------------------------------------------------------------------
+    @classmethod
+    def starts_task(cls, name, **task_kwargs):
+
+        def starts_task_decorator(func):
+
+            @wraps(func)
+            def starts_task_wrapper(self, request, *args, **kwargs):
+                bgtask = self.start_bgtask(name, **task_kwargs)
+                result = func(self, request, *args, bgtask=bgtask, **kwargs)
+                self.message_user(request, f"Dispatched task {name}", INFO)
+
+            func.bgtask_name = name
+
+            return starts_task_wrapper
+
+        return starts_task_decorator
+
+    # ----------------------------------------------------------------------------------------------
     # API for subclasses
     # ----------------------------------------------------------------------------------------------
     def start_bgtask(self, name, **kwargs):
         bgtask = BackgroundTask.objects.create(
             name=name,
             namespace=self._bgtask_namespace,
             **kwargs,
@@ -37,35 +60,53 @@
     # ----------------------------------------------------------------------------------------------
     # Internal functions
     # ----------------------------------------------------------------------------------------------
     @property
     def _bgtask_namespace(self):
         return type(self).__module__ + "." + type(self).__name__
 
+    @staticmethod
+    def _extract_bgtask_name_from_admin_action(action):
+        # recurse through the potentially wrapped action until we find one that declares
+        # the bgtask_name
+        next_action = action
+        while True:
+            if hasattr(next_action, "bgtask_name"):
+                return next_action.bgtask_name
+
+            if not hasattr(next_action, "__wrapped__"):
+                return None
+
+            next_action = next_action.__wrapped__
+
     def _admin_bg_tasks(self, request):
         task_name_to_desc = {}
         for action, action_name, action_description in self.get_actions(request).values():
-            if hasattr(action, "bgtask_name"):
-                task_name_to_desc[action.bgtask_name] = action_description
+            bgtask_name = self._extract_bgtask_name_from_admin_action(action)
+            if bgtask_name is not None:
+                task_name_to_desc[bgtask_name] = action_description
 
         for name in getattr(self, "bgtask_names", []):
             task_name_to_desc[name] = name
 
         if not task_name_to_desc:
             return BackgroundTask.objects.none()
 
         bgts = list(
             BackgroundTask.objects.filter(
                 name__in=task_name_to_desc, namespace=self._bgtask_namespace
             )
             .filter(
-                Q(state=BackgroundTask.STATES.running)
+                (
+                    Q(state=BackgroundTask.STATES.running)
+                    & Q(started_at__gt=timezone.now() - timedelta(days=1))
+                )
                 | (
                     ~Q(state=BackgroundTask.STATES.not_started)
-                    & Q(completed_at__gt=timezone.now() - timedelta(minutes=30))
+                    & Q(completed_at__gt=timezone.now() - timedelta(hours=2))
                 )
             )
             .order_by("-started_at")
         )
         for bgt in bgts:
             bgt.admin_description = task_name_to_desc[bgt.name]
```

### Comparing `django_admin_background_task-0.2.0/bgtask/models.py` & `django_admin_background_task-0.3.0/bgtask/models.py`

 * *Files identical despite different names*

### Comparing `django_admin_background_task-0.2.0/bgtask/static/bgtask/js/bgtask-once.js` & `django_admin_background_task-0.3.0/bgtask/static/bgtask/js/bgtask-once.js`

 * *Files identical despite different names*

### Comparing `django_admin_background_task-0.2.0/bgtask/static/bgtask/js/bgtask.js` & `django_admin_background_task-0.3.0/bgtask/static/bgtask/js/bgtask.js`

 * *Files 10% similar despite different names*

#### js-beautify {}

```diff
@@ -10,14 +10,41 @@
 
 const OUT_OF_DATE_PERIOD_S = 20;
 const REFRESH_PERIOD_MS = 5000;
 const TIME_TO_REDUCED_REFRESH_PERIOD_S = 300;
 const REDUCED_REFRESH_PERIOD_S = 60;
 const PROGRESS_REFRESH_MS = 100;
 
+function millisecondsToTimeAgoString(ms) {
+    const seconds = Math.floor(ms / 1000);
+    const minutes = Math.floor(seconds / 60);
+    const hours = Math.floor(minutes / 60);
+    const days = Math.floor(hours / 24);
+
+    if (days > 0) {
+        if (days === 1) {
+            return `${days} day, ${hours % 24} hours ago`;
+        }
+        return `${days} days ago`;
+    }
+    if (hours > 0) {
+        if (hours === 1) {
+            return `${hours} hour, ${minutes % 60} minutes ago`;
+        }
+        return `${hours} hours ago`;
+    }
+    if (minutes > 0) {
+        if (minutes === 1) {
+            return `${minutes} minute, ${seconds % 60} seconds ago`;
+        }
+        return `${minutes} minutes ago`;
+    }
+    return `${seconds} seconds ago`;
+}
+
 // -------------------------------------------------------------------------------------------------
 // Generic live-looking progress bar manager.
 // -------------------------------------------------------------------------------------------------
 class ProgressState {
     constructor(element, {
         value,
         max
@@ -149,27 +176,33 @@
     }
 
     attachToPoller(poller) {
         poller.monitorTask(this.taskId, task => this.updateFromTask(task));
     }
 
     updateFromTask(task) {
-        // console.log(`TaskProgressDiv.updateFromTask`, task);
         this.div.title = "";
 
         switch (task.state) {
             case "partial_success":
                 this._hideProgress();
                 this._showState();
                 this._addTitle("Some errors occurred");
                 break;
             case "failed":
                 this._hideProgress();
                 this._showState();
-                this._addTitle("Task failed");
+                let title = "Task failed";
+                for (const error of task.errors) {
+                    if (error.traceback) {
+                        title = `${title}\n${error.traceback}\n\n${error.error_message}`;
+                        break;
+                    }
+                }
+                this._addTitle(title);
                 break;
             case "success":
                 this._hideProgress();
                 this._showState();
                 this._addTitle("Task succeeded");
                 break;
             case "not_started":
@@ -219,14 +252,34 @@
     }
     _showState() {
         this.stateEle.style.display = null;
     }
 }
 
 // -------------------------------------------------------------------------------------------------
+// Manage an element which just shows one field from the task
+// -------------------------------------------------------------------------------------------------
+class TaskFieldElement {
+    constructor(element, fieldName, task) {
+        this.taskId = task.id;
+        this.element = element;
+        this.fieldName = fieldName;
+        this.updateFromTask(task);
+    }
+
+    attachToPoller(poller) {
+        poller.monitorTask(this.taskId, task => this.updateFromTask(task));
+    }
+
+    updateFromTask(task) {
+        this.element.innerHTML = task[this.fieldName];
+    }
+}
+
+// -------------------------------------------------------------------------------------------------
 // Manage a task detail div
 // -------------------------------------------------------------------------------------------------
 class BGTaskDetailViewDiv {
     constructor(div, task, poller) {
         this.taskId = task.id;
         this.div = div;
         this.progressDiv = new TaskProgressDiv(
@@ -312,14 +365,22 @@
         this.mostRecentUpdate = null;
     }
 
     static instances = {};
 
     static normalizeTask(task) {
         task.updated = new Date(task.updated);
+
+        if (task.completed_at !== null) {
+            task.completed_at = new Date(task.completed_at);
+            const completedTimeAgoMS = Date.now() - task.completed_at.getTime();
+            task.completed_at_time_ago = millisecondsToTimeAgoString(completedTimeAgoMS);
+        } else {
+            task.completed_at_time_ago = "–";
+        }
     }
 
     static sharedInstance(baseURL) {
         if (BGTaskPoller.instances[baseURL] === undefined) {
             BGTaskPoller.instances[baseURL] = new BGTaskPoller(baseURL);
         }
         return BGTaskPoller.instances[baseURL];
@@ -372,15 +433,17 @@
     _sendPoll() {
         this.intvl = null;
         const req = new XMLHttpRequest();
         const self = this;
         req.addEventListener("load", function() {
             self._receivePoll(this);
         });
-        const url = `${this.baseURL}?tasks=${Object.keys(this.taskCallbacks).join(",")}`;
+        const taskIds = Object.keys(this.taskCallbacks).join(",");
+        const url = `${this.baseURL}?tasks=${taskIds}`;
+        console.log(`Poll for tasks ${taskIds}`);
         req.open("GET", url);
         req.setRequestHeader('Accept', 'application/json');
         req.send();
     }
     _receivePoll(response) {
         var tasks;
         try {
```

### Comparing `django_admin_background_task-0.2.0/bgtask/templates/bgtask/admin/change_list.html` & `django_admin_background_task-0.3.0/bgtask/templates/bgtask/admin/change_list.html`

 * *Files 13% similar despite different names*

```diff
@@ -4,27 +4,27 @@
 {% block extrastyle %}
 {{ block.super }}
 <link rel="stylesheet" type="text/css" href="{% static "admin/css/forms.css" %}">
 {% endblock %}
 
 {% block object-tools %}
 {{ block.super }}
-<div>
+<div style="margin-bottom: 10px;">
   <h3>Action background tasks</h3>
   {% if not admin_bg_tasks|length %}
   <p class="help" style="font-style: italic;">No recent background tasks</p>
   {% else %}
   <table>
     <thead>
       <tr><th>Task name</th><th>Started</th><th>Finished</th><th>Status</th></tr>
     </thead>
     <tbody>
       {% for bgt in admin_bg_tasks %}
       {% with bgtask=bgt.task_dict %}
-      <tr class="bgtask-row"><td><a href="{% url 'admin:bgtask_backgroundtask_change' bgtask.id %}">{{ bgt.admin_description }}</a></td><td>{{ bgt.started_at|timesince }} ago</td><td>{% if bgt.completed_at %}{{ bgt.completed_at|timesince }} ago{% else %}–{% endif %}</td><td>
+      <tr class="bgtask-row"><td><a href="{% url 'admin:bgtask_backgroundtask_change' bgtask.id %}">{{ bgt.admin_description }}</a></td><td>{{ bgt.started_at|timesince }} ago</td><td>{% include "bgtask/bg_completed_column.html" %}</td><td>
       {% include "bgtask/bg_changelist_status_column.html" %}</td></tr>
       {% endwith %}
       {% endfor %}
     </tbody>
   </table>
   {% endif %}
 </div>
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

#### html2text {}

```diff
@@ -1,15 +1,14 @@
 {% extends "admin/change_list.html" %} {% load static %} {% block extrastyle %}
 {{ block.super }}
 }"> {% endblock %} {% block object-tools %} {{ block.super }}
 ******** AAccttiioonn bbaacckkggrroouunndd ttaasskkss ********
 {% if not admin_bg_tasks|length %}
 No recent background tasks
 {% else %}
-TTaasskk nnaammee             SSttaarrtteedd                  FFiinniisshheedd                   SSttaattuuss
-_{                     {                        {% if bgt.completed_at %}{
-_{                     {                        {                          {% include "bgtask/
-_b_g_t_._a_d_m_i_n___d_e_s_c_r_i_p_t_i_o_n bgt.started_at|timesince bgt.completed_at|timesince bg_changelist_status_column.html"
-_}_}                    }} ago                   }} ago{% else %}â{%      %}
-                                               endif %}
+TTaasskk nnaammee             SSttaarrtteedd                  FFiinniisshheedd                  SSttaattuuss
+_{                     {                        {% include "bgtask/       {% include "bgtask/
+_{                     {                        bg_completed_column.html" bg_changelist_status_column.html"
+_b_g_t_._a_d_m_i_n___d_e_s_c_r_i_p_t_i_o_n bgt.started_at|timesince %}                        %}
+_}_}                    }} ago
 {% endif %}
 {% endblock %}
```

### Comparing `django_admin_background_task-0.2.0/bgtask/templates/bgtask/bg_changelist_status_column.html` & `django_admin_background_task-0.3.0/bgtask/templates/bgtask/bg_changelist_status_column.html`

 * *Files 8% similar despite different names*

```diff
@@ -2,19 +2,15 @@
 {% if not bgtask %}
 -
 {% else %}
 {% with initialTasksJsonId="initialTasksJson-"|add:bgtask.id %}
 {{ bgtask|json_script:initialTasksJsonId }}
 {% endwith %}
 <script src="{% static 'bgtask/js/bgtask-once.js' %}"></script>
-{% if bgtask.acted_on_object_id %}
-<a href="{% url 'bgtask:tasks' %}?object_id={{bgtask.acted_on_object_id}}">
-{% else %}
 <a href="{% url 'admin:bgtask_backgroundtask_change' bgtask.id %}">
-{% endif %}
     <div id="bgtask-column-{{ bgtask.id }}">
         {% include 'bgtask/progress.html' %}
     </div>
 </a>
 <script>
 (() => {
     const poller = BGTaskPoller.sharedInstance("{% url 'bgtask:tasks' %}");
```

#### html2text {}

```diff
@@ -1,8 +1,5 @@
 {% load static %} {% if not bgtask %} - {% else %} {% with
 initialTasksJsonId="initialTasksJson-"|add:bgtask.id %} {{ bgtask|json_script:
 initialTasksJsonId }} {% endwith %}
-{% if bgtask.acted_on_object_id %}
-_{_%_ _e_l_s_e_ _%_}
-_{_%_ _e_n_d_i_f_ _%_}
 _{_%_ _i_n_c_l_u_d_e_ _'_b_g_t_a_s_k_/_p_r_o_g_r_e_s_s_._h_t_m_l_'_ _%_}
 {% endif %}
```

### Comparing `django_admin_background_task-0.2.0/bgtask/templates/bgtask/bgtask_view.html` & `django_admin_background_task-0.3.0/bgtask/templates/bgtask/bgtask_view.html`

 * *Files identical despite different names*

### Comparing `django_admin_background_task-0.2.0/bgtask/tests/test_bgtask.py` & `django_admin_background_task-0.3.0/bgtask/tests/test_bgtask.py`

 * *Files identical despite different names*

### Comparing `django_admin_background_task-0.2.0/bgtask/views.py` & `django_admin_background_task-0.3.0/bgtask/views.py`

 * *Files identical despite different names*

### Comparing `django_admin_background_task-0.2.0/pyproject.toml` & `django_admin_background_task-0.3.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "django-admin-background-task"
-version = "0.2.0"
+version = "0.3.0"
 description = "A set of tools for django apps to persist and monitor the status of background tasks"
 authors = [
     "David Park <david@greenparksoftware.co.uk>",
 ]
 readme = "README.md"
 license = "Apache-2.0"
 repository = "https://github.com/daphtdazz/django-bgtask"
```

### Comparing `django_admin_background_task-0.2.0/PKG-INFO` & `django_admin_background_task-0.3.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-admin-background-task
-Version: 0.2.0
+Version: 0.3.0
 Summary: A set of tools for django apps to persist and monitor the status of background tasks
 Home-page: https://github.com/daphtdazz/django-bgtask
 License: Apache-2.0
 Author: David Park
 Author-email: david@greenparksoftware.co.uk
 Requires-Python: >=3.11,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
```

