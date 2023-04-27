# Comparing `tmp/cognitivefactory-interactive-clustering-gui-0.4.0.tar.gz` & `tmp/cognitivefactory-interactive-clustering-gui-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cognitivefactory-interactive-clustering-gui-0.4.0.tar", last modified: Thu Sep  1 09:47:01 2022, max compression
+gzip compressed data, was "cognitivefactory-interactive-clustering-gui-0.4.1.tar", last modified: Thu Apr 27 09:32:58 2023, max compression
```

## Comparing `cognitivefactory-interactive-clustering-gui-0.4.0.tar` & `cognitivefactory-interactive-clustering-gui-0.4.1.tar`

### file list

```diff
@@ -1,653 +1,653 @@
--rw-rw-rw-   0        0        0    22748 2022-08-18 15:35:45.547399 cognitivefactory-interactive-clustering-gui-0.4.0/LICENSE.md
--rw-rw-rw-   0        0        0     4228 2022-09-01 07:02:38.869574 cognitivefactory-interactive-clustering-gui-0.4.0/pyproject.toml
--rw-rw-rw-   0        0        0     6051 2022-08-31 15:10:46.280755 cognitivefactory-interactive-clustering-gui-0.4.0/README.md
--rw-rw-rw-   0        0        0      197 2022-08-22 12:28:57.751742 cognitivefactory-interactive-clustering-gui-0.4.0/src/cognitivefactory/interactive_clustering_gui/__init__.py
--rw-rw-rw-   0        0        0     1055 2022-08-26 11:33:58.069540 cognitivefactory-interactive-clustering-gui-0.4.0/src/cognitivefactory/interactive_clustering_gui/__main__.py
--rw-rw-rw-   0        0        0   141215 2022-08-31 15:20:16.485964 cognitivefactory-interactive-clustering-gui-0.4.0/src/cognitivefactory/interactive_clustering_gui/app.py
--rw-rw-rw-   0        0        0    34573 2022-08-25 09:39:54.622436 cognitivefactory-interactive-clustering-gui-0.4.0/src/cognitivefactory/interactive_clustering_gui/backgroundtasks.py
--rw-rw-rw-   0        0        0     3495 2022-08-26 15:43:51.280254 cognitivefactory-interactive-clustering-gui-0.4.0/src/cognitivefactory/interactive_clustering_gui/cli.py
--rw-rw-rw-   0        0        0     6527 2022-03-10 09:47:37.411388 cognitivefactory-interactive-clustering-gui-0.4.0/src/cognitivefactory/interactive_clustering_gui/css/new_styles.css
--rw-rw-rw-   0        0        0    13550 2022-07-29 09:36:01.515330 cognitivefactory-interactive-clustering-gui-0.4.0/src/cognitivefactory/interactive_clustering_gui/css/styles.css
--rw-rw-rw-   0        0        0     4162 2022-07-06 09:25:12.810974 cognitivefactory-interactive-clustering-gui-0.4.0/src/cognitivefactory/interactive_clustering_gui/html/_base.html
--rw-rw-rw-   0        0        0    10046 2022-02-07 09:06:45.352415 cognitivefactory-interactive-clustering-gui-0.4.0/src/cognitivefactory/interactive_clustering_gui/html/analytics.html
--rw-rw-rw-   0        0        0    19323 2022-08-31 14:58:43.438900 cognitivefactory-interactive-clustering-gui-0.4.0/src/cognitivefactory/interactive_clustering_gui/html/constraint_annotation.html
--rw-rw-rw-   0        0        0    18201 2022-08-31 14:59:04.148342 cognitivefactory-interactive-clustering-gui-0.4.0/src/cognitivefactory/interactive_clustering_gui/html/constraints.html
--rw-rw-rw-   0        0        0      635 2022-07-19 15:10:00.770489 cognitivefactory-interactive-clustering-gui-0.4.0/src/cognitivefactory/interactive_clustering_gui/html/error.html
--rw-rw-rw-   0        0        0      600 2022-08-31 15:01:20.049462 cognitivefactory-interactive-clustering-gui-0.4.0/src/cognitivefactory/interactive_clustering_gui/html/help.html
--rw-rw-rw-   0        0        0    15608 2022-08-31 14:59:25.146710 cognitivefactory-interactive-clustering-gui-0.4.0/src/cognitivefactory/interactive_clustering_gui/html/project_home.html
--rw-rw-rw-   0        0        0     8971 2022-08-30 12:16:12.152401 cognitivefactory-interactive-clustering-gui-0.4.0/src/cognitivefactory/interactive_clustering_gui/html/projects_listing.html
--rw-rw-rw-   0        0        0    35499 2022-07-26 11:22:40.014591 cognitivefactory-interactive-clustering-gui-0.4.0/src/cognitivefactory/interactive_clustering_gui/html/settings.html
--rw-rw-rw-   0        0        0    13102 2022-08-31 14:59:42.321939 cognitivefactory-interactive-clustering-gui-0.4.0/src/cognitivefactory/interactive_clustering_gui/html/texts.html
--rw-rw-rw-   0        0        0    14661 2022-06-03 12:53:45.394276 cognitivefactory-interactive-clustering-gui-0.4.0/src/cognitivefactory/interactive_clustering_gui/html/welcome.html
--rw-rw-rw-   0        0        0     5561 2022-07-06 07:23:29.966040 cognitivefactory-interactive-clustering-gui-0.4.0/src/cognitivefactory/interactive_clustering_gui/js/analytics.js
--rw-rw-rw-   0        0        0    17011 2022-07-07 11:36:32.036053 cognitivefactory-interactive-clustering-gui-0.4.0/src/cognitivefactory/interactive_clustering_gui/js/annotation.js
--rw-rw-rw-   0        0        0     1133 2022-06-08 14:26:13.573749 cognitivefactory-interactive-clustering-gui-0.4.0/src/cognitivefactory/interactive_clustering_gui/js/collapsing.js
--rw-rw-rw-   0        0        0    11925 2022-08-31 14:52:17.264788 cognitivefactory-interactive-clustering-gui-0.4.0/src/cognitivefactory/interactive_clustering_gui/js/constraints.js
--rw-rw-rw-   0        0        0     3544 2022-08-31 14:50:40.593212 cognitivefactory-interactive-clustering-gui-0.4.0/src/cognitivefactory/interactive_clustering_gui/js/goto.js
--rw-rw-rw-   0        0        0     3103 2022-07-07 06:56:56.317968 cognitivefactory-interactive-clustering-gui-0.4.0/src/cognitivefactory/interactive_clustering_gui/js/projects.js
--rw-rw-rw-   0        0        0     8590 2022-07-29 09:12:47.093532 cognitivefactory-interactive-clustering-gui-0.4.0/src/cognitivefactory/interactive_clustering_gui/js/projects_listing.js
--rw-rw-rw-   0        0        0    19918 2022-06-08 12:33:49.604197 cognitivefactory-interactive-clustering-gui-0.4.0/src/cognitivefactory/interactive_clustering_gui/js/settings.js
--rw-rw-rw-   0        0        0    36228 2022-08-31 15:22:35.389593 cognitivefactory-interactive-clustering-gui-0.4.0/src/cognitivefactory/interactive_clustering_gui/js/status.js
--rw-rw-rw-   0        0        0     7167 2022-06-24 15:41:20.664796 cognitivefactory-interactive-clustering-gui-0.4.0/src/cognitivefactory/interactive_clustering_gui/js/tasks.js
--rw-rw-rw-   0        0        0      100 2022-07-21 16:16:51.353096 cognitivefactory-interactive-clustering-gui-0.4.0/src/cognitivefactory/interactive_clustering_gui/models/__init__.py
--rw-rw-rw-   0        0        0     2090 2022-08-23 12:17:43.082363 cognitivefactory-interactive-clustering-gui-0.4.0/src/cognitivefactory/interactive_clustering_gui/models/queries.py
--rw-rw-rw-   0        0        0    27380 2022-08-22 15:59:06.845649 cognitivefactory-interactive-clustering-gui-0.4.0/src/cognitivefactory/interactive_clustering_gui/models/settings.py
--rw-rw-rw-   0        0        0    14411 2022-08-22 15:59:06.844652 cognitivefactory-interactive-clustering-gui-0.4.0/src/cognitivefactory/interactive_clustering_gui/models/states.py
--rw-rw-rw-   0        0        0        0 2022-08-18 15:35:45.642146 cognitivefactory-interactive-clustering-gui-0.4.0/src/cognitivefactory/interactive_clustering_gui/py.typed
--rw-rw-rw-   0        0        0    39169 2022-02-01 13:28:39.443263 cognitivefactory-interactive-clustering-gui-0.4.0/src/cognitivefactory/interactive_clustering_gui/resources/diagrams/example_clustering.png
--rw-rw-rw-   0        0        0    25318 2022-02-01 13:32:14.299349 cognitivefactory-interactive-clustering-gui-0.4.0/src/cognitivefactory/interactive_clustering_gui/resources/diagrams/example_constrained_clustering.png
--rw-rw-rw-   0        0        0    12842 2022-02-01 13:20:59.849702 cognitivefactory-interactive-clustering-gui-0.4.0/src/cognitivefactory/interactive_clustering_gui/resources/diagrams/example_constraints.png
--rw-rw-rw-   0        0        0    10956 2022-02-03 08:57:31.044494 cognitivefactory-interactive-clustering-gui-0.4.0/src/cognitivefactory/interactive_clustering_gui/resources/diagrams/example_constraints_conflict.png
--rw-rw-rw-   0        0        0    10672 2022-02-03 08:58:08.867236 cognitivefactory-interactive-clustering-gui-0.4.0/src/cognitivefactory/interactive_clustering_gui/resources/diagrams/example_constraints_inference_cannot_link.png
--rw-rw-rw-   0        0        0     7018 2022-02-03 08:57:54.997255 cognitivefactory-interactive-clustering-gui-0.4.0/src/cognitivefactory/interactive_clustering_gui/resources/diagrams/example_constraints_inference_must_link.png
--rw-rw-rw-   0        0        0    54984 2022-02-01 14:48:40.372500 cognitivefactory-interactive-clustering-gui-0.4.0/src/cognitivefactory/interactive_clustering_gui/resources/diagrams/example_sampling.png
--rw-rw-rw-   0        0        0   196607 2022-02-01 17:32:29.088734 cognitivefactory-interactive-clustering-gui-0.4.0/src/cognitivefactory/interactive_clustering_gui/resources/diagrams/interactive_clustering.png
--rw-rw-rw-   0        0        0    20973 2021-10-20 12:37:23.353701 cognitivefactory-interactive-clustering-gui-0.4.0/src/cognitivefactory/interactive_clustering_gui/resources/logos/github.png
--rw-rw-rw-   0        0        0    12395 2022-07-06 08:49:07.035648 cognitivefactory-interactive-clustering-gui-0.4.0/src/cognitivefactory/interactive_clustering_gui/resources/logos/interactive_clustering_black.png
--rw-rw-rw-   0        0        0     5648 2022-07-06 08:12:20.405379 cognitivefactory-interactive-clustering-gui-0.4.0/src/cognitivefactory/interactive_clustering_gui/resources/logos/interactive_clustering_blue.png
--rw-rw-rw-   0        0        0     5645 2022-07-06 08:14:49.966463 cognitivefactory-interactive-clustering-gui-0.4.0/src/cognitivefactory/interactive_clustering_gui/resources/logos/interactive_clustering_gray_1.png
--rw-rw-rw-   0        0        0     5415 2022-07-06 08:14:15.093499 cognitivefactory-interactive-clustering-gui-0.4.0/src/cognitivefactory/interactive_clustering_gui/resources/logos/interactive_clustering_gray_2.png
--rw-rw-rw-   0        0        0    16485 2022-07-06 08:14:00.677811 cognitivefactory-interactive-clustering-gui-0.4.0/src/cognitivefactory/interactive_clustering_gui/resources/logos/interactive_clustering_pink.png
--rw-rw-rw-   0        0        0    13258 2021-10-20 12:37:23.359688 cognitivefactory-interactive-clustering-gui-0.4.0/src/cognitivefactory/interactive_clustering_gui/resources/logos/interactive_clustering_white.png
--rw-rw-rw-   0        0        0      196 2022-08-22 15:59:06.825664 cognitivefactory-interactive-clustering-gui-0.4.0/tests/__init__.py
--rw-rw-rw-   0        0        0     3249 2022-08-26 14:31:56.269726 cognitivefactory-interactive-clustering-gui-0.4.0/tests/conftest.py
--rw-rw-rw-   0        0        0        2 2022-07-11 12:07:21.312463 cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/0a_INITIALIZATION_WITHOUT_MODELIZATION/clustering.json
--rw-rw-rw-   0        0        0        2 2022-07-11 12:07:21.271572 cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/0a_INITIALIZATION_WITHOUT_MODELIZATION/constraints.json
--rw-rw-rw-   0        0        0      144 2022-07-11 12:24:22.394714 cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/0a_INITIALIZATION_WITHOUT_MODELIZATION/metadata.json
--rw-rw-rw-   0        0        0     3045 2022-07-11 12:07:21.303486 cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/0a_INITIALIZATION_WITHOUT_MODELIZATION/modelization.json
--rw-rw-rw-   0        0        0        2 2022-07-11 12:07:21.309471 cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/0a_INITIALIZATION_WITHOUT_MODELIZATION/sampling.json
--rw-rw-rw-   0        0        0      696 2022-07-11 12:13:45.311609 cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/0a_INITIALIZATION_WITHOUT_MODELIZATION/settings.json
--rw-rw-rw-   0        0        0       99 2022-07-11 12:07:21.264592 cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/0a_INITIALIZATION_WITHOUT_MODELIZATION/status.json
--rw-rw-rw-   0        0        0     6659 2022-07-11 12:07:21.267583 cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/0a_INITIALIZATION_WITHOUT_MODELIZATION/texts.json
--rw-rw-rw-   0        0        0        2 2022-07-11 12:07:21.312463 cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/0b_INITIALIZATION_WITH_PENDING_MODELIZATION/clustering.json
--rw-rw-rw-   0        0        0        2 2022-07-11 12:07:21.271572 cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/0b_INITIALIZATION_WITH_PENDING_MODELIZATION/constraints.json
--rw-rw-rw-   0        0        0      149 2022-07-25 14:28:29.853559 cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/0b_INITIALIZATION_WITH_PENDING_MODELIZATION/metadata.json
--rw-rw-rw-   0        0        0     3045 2022-07-11 12:07:21.303486 cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/0b_INITIALIZATION_WITH_PENDING_MODELIZATION/modelization.json
--rw-rw-rw-   0        0        0        2 2022-07-11 12:07:21.309471 cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/0b_INITIALIZATION_WITH_PENDING_MODELIZATION/sampling.json
--rw-rw-rw-   0        0        0      696 2022-07-11 12:13:45.311609 cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/0b_INITIALIZATION_WITH_PENDING_MODELIZATION/settings.json
--rw-rw-rw-   0        0        0      198 2022-08-23 08:03:11.312599 cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/0b_INITIALIZATION_WITH_PENDING_MODELIZATION/status.json
--rw-rw-rw-   0        0        0     6659 2022-07-11 12:07:21.267583 cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/0b_INITIALIZATION_WITH_PENDING_MODELIZATION/texts.json
--rw-rw-rw-   0        0        0        2 2022-07-11 12:07:21.312463 cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/0c_INITIALIZATION_WITH_WORKING_MODELIZATION/clustering.json
--rw-rw-rw-   0        0        0        2 2022-07-11 12:07:21.271572 cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/0c_INITIALIZATION_WITH_WORKING_MODELIZATION/constraints.json
--rw-rw-rw-   0        0        0      149 2022-07-25 14:29:48.166071 cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/0c_INITIALIZATION_WITH_WORKING_MODELIZATION/metadata.json
--rw-rw-rw-   0        0        0     3045 2022-07-11 12:07:21.303486 cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/0c_INITIALIZATION_WITH_WORKING_MODELIZATION/modelization.json
--rw-rw-rw-   0        0        0        2 2022-07-11 12:07:21.309471 cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/0c_INITIALIZATION_WITH_WORKING_MODELIZATION/sampling.json
--rw-rw-rw-   0        0        0      696 2022-07-11 12:13:45.311609 cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/0c_INITIALIZATION_WITH_WORKING_MODELIZATION/settings.json
--rw-rw-rw-   0        0        0      175 2022-08-23 08:03:11.377428 cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/0c_INITIALIZATION_WITH_WORKING_MODELIZATION/status.json
--rw-rw-rw-   0        0        0     6659 2022-07-11 12:07:21.267583 cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/0c_INITIALIZATION_WITH_WORKING_MODELIZATION/texts.json
--rw-rw-rw-   0        0        0        2 2022-07-11 12:07:21.312463 cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/0d_CLUSTERING_TODO/clustering.json
--rw-rw-rw-   0        0        0        2 2022-07-11 12:10:27.067191 cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/0d_CLUSTERING_TODO/constraints.json
--rw-rw-rw-   0        0        0     1880 2022-08-23 13:18:44.586771 cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/0d_CLUSTERING_TODO/constraints_manager.pkl
--rw-rw-rw-   0        0        0      124 2022-07-25 14:32:47.239376 cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/0d_CLUSTERING_TODO/metadata.json
--rw-rw-rw-   0        0        0     3045 2022-07-11 12:10:27.509082 cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/0d_CLUSTERING_TODO/modelization.json
--rw-rw-rw-   0        0        0        2 2022-07-11 12:07:21.309471 cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/0d_CLUSTERING_TODO/sampling.json
--rw-rw-rw-   0        0        0      696 2022-07-11 12:13:54.079094 cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/0d_CLUSTERING_TODO/settings.json
--rw-rw-rw-   0        0        0       79 2022-07-11 12:10:27.524042 cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/0d_CLUSTERING_TODO/status.json
--rw-rw-rw-   0        0        0     6513 2022-07-11 12:10:23.869094 cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/0d_CLUSTERING_TODO/texts.json
--rw-rw-rw-   0        0        0     5825 2022-07-11 12:10:24.327037 cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/0d_CLUSTERING_TODO/vectors.pkl
--rw-rw-rw-   0        0        0     2106 2022-07-11 12:10:25.284783 cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/0d_CLUSTERING_TODO/vectors_2D.json
--rw-rw-rw-   0        0        0     2904 2022-07-11 12:10:26.615845 cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/0d_CLUSTERING_TODO/vectors_3D.json
--rw-rw-rw-   0        0        0        2 2022-07-11 12:07:21.312463 cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/0e_CLUSTERING_PENDING/clustering.json
--rw-rw-rw-   0        0        0        2 2022-07-11 12:10:27.067191 cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/0e_CLUSTERING_PENDING/constraints.json
--rw-rw-rw-   0        0        0     1880 2022-08-23 13:18:41.974764 cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/0e_CLUSTERING_PENDING/constraints_manager.pkl
--rw-rw-rw-   0        0        0      127 2022-07-25 14:31:40.122180 cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/0e_CLUSTERING_PENDING/metadata.json
--rw-rw-rw-   0        0        0     3045 2022-07-11 12:10:27.509082 cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/0e_CLUSTERING_PENDING/modelization.json
--rw-rw-rw-   0        0        0        2 2022-07-11 12:07:21.309471 cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/0e_CLUSTERING_PENDING/sampling.json
--rw-rw-rw-   0        0        0      696 2022-07-11 12:13:34.463283 cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/0e_CLUSTERING_PENDING/settings.json
--rw-rw-rw-   0        0        0      177 2022-08-23 08:03:11.373438 cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/0e_CLUSTERING_PENDING/status.json
--rw-rw-rw-   0        0        0     6513 2022-07-11 12:10:23.869094 cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/0e_CLUSTERING_PENDING/texts.json
--rw-rw-rw-   0        0        0     5825 2022-07-11 12:10:24.327037 cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/0e_CLUSTERING_PENDING/vectors.pkl
--rw-rw-rw-   0        0        0     2106 2022-07-11 12:10:25.284783 cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/0e_CLUSTERING_PENDING/vectors_2D.json
--rw-rw-rw-   0        0        0     2904 2022-07-11 12:10:26.615845 cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/0e_CLUSTERING_PENDING/vectors_3D.json
--rw-rw-rw-   0        0        0        2 2022-07-11 12:07:21.312463 cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/0f_CLUSTERING_WORKING/clustering.json
--rw-rw-rw-   0        0        0        2 2022-07-11 12:10:27.067191 cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/0f_CLUSTERING_WORKING/constraints.json
--rw-rw-rw-   0        0        0     1880 2022-08-23 13:18:41.982747 cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/0f_CLUSTERING_WORKING/constraints_manager.pkl
--rw-rw-rw-   0        0        0      127 2022-07-25 14:34:10.768459 cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/0f_CLUSTERING_WORKING/metadata.json
--rw-rw-rw-   0        0        0     3045 2022-07-11 12:10:27.509082 cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/0f_CLUSTERING_WORKING/modelization.json
--rw-rw-rw-   0        0        0        2 2022-07-11 12:07:21.309471 cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/0f_CLUSTERING_WORKING/sampling.json
--rw-rw-rw-   0        0        0      696 2022-07-11 12:13:34.463283 cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/0f_CLUSTERING_WORKING/settings.json
--rw-rw-rw-   0        0        0      149 2022-08-23 08:03:11.366457 cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/0f_CLUSTERING_WORKING/status.json
--rw-rw-rw-   0        0        0     6513 2022-07-11 12:10:23.869094 cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/0f_CLUSTERING_WORKING/texts.json
--rw-rw-rw-   0        0        0     5825 2022-07-11 12:10:24.327037 cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/0f_CLUSTERING_WORKING/vectors.pkl
--rw-rw-rw-   0        0        0     2106 2022-07-11 12:10:25.284783 cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/0f_CLUSTERING_WORKING/vectors_2D.json
--rw-rw-rw-   0        0        0     2904 2022-07-11 12:10:26.615845 cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/0f_CLUSTERING_WORKING/vectors_3D.json
--rw-rw-rw-   0        0        0      444 2022-07-11 12:14:11.348217 cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/0g_ITERATION_END/clustering.json
--rw-rw-rw-   0        0        0        2 2022-07-11 12:10:27.067191 cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/0g_ITERATION_END/constraints.json
--rw-rw-rw-   0        0        0     1880 2022-08-23 13:18:41.988728 cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/0g_ITERATION_END/constraints_manager.pkl
--rw-rw-rw-   0        0        0      122 2022-07-25 14:34:47.905746 cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/0g_ITERATION_END/metadata.json
--rw-rw-rw-   0        0        0     3045 2022-07-11 12:10:27.509082 cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/0g_ITERATION_END/modelization.json
--rw-rw-rw-   0        0        0        2 2022-07-11 12:07:21.309471 cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/0g_ITERATION_END/sampling.json
--rw-rw-rw-   0        0        0      696 2022-07-11 12:13:34.463283 cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/0g_ITERATION_END/settings.json
--rw-rw-rw-   0        0        0       77 2022-07-11 12:14:11.366169 cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/0g_ITERATION_END/status.json
--rw-rw-rw-   0        0        0     6513 2022-07-11 12:10:23.869094 cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/0g_ITERATION_END/texts.json
--rw-rw-rw-   0        0        0     5825 2022-07-11 12:10:24.327037 cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/0g_ITERATION_END/vectors.pkl
--rw-rw-rw-   0        0        0     2106 2022-07-11 12:10:25.284783 cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/0g_ITERATION_END/vectors_2D.json
--rw-rw-rw-   0        0        0     2904 2022-07-11 12:10:26.615845 cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/0g_ITERATION_END/vectors_3D.json
--rw-rw-rw-   0        0        0      444 2022-07-11 12:14:11.348217 cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/1a_SAMPLING_TODO/clustering.json
--rw-rw-rw-   0        0        0        2 2022-07-11 12:10:27.067191 cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/1a_SAMPLING_TODO/constraints.json
--rw-rw-rw-   0        0        0     1880 2022-08-23 13:18:41.994713 cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/1a_SAMPLING_TODO/constraints_manager.pkl
--rw-rw-rw-   0        0        0      122 2022-07-11 12:26:59.431426 cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/1a_SAMPLING_TODO/metadata.json
--rw-rw-rw-   0        0        0     3045 2022-07-11 12:10:27.509082 cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/1a_SAMPLING_TODO/modelization.json
--rw-rw-rw-   0        0        0        2 2022-07-11 12:07:21.309471 cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/1a_SAMPLING_TODO/sampling.json
--rw-rw-rw-   0        0        0     1580 2022-07-11 12:18:44.031863 cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/1a_SAMPLING_TODO/settings.json
--rw-rw-rw-   0        0        0       77 2022-07-11 12:18:44.033857 cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/1a_SAMPLING_TODO/status.json
--rw-rw-rw-   0        0        0     6513 2022-07-11 12:10:23.869094 cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/1a_SAMPLING_TODO/texts.json
--rw-rw-rw-   0        0        0     5825 2022-07-11 12:10:24.327037 cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/1a_SAMPLING_TODO/vectors.pkl
--rw-rw-rw-   0        0        0     2106 2022-07-11 12:10:25.284783 cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/1a_SAMPLING_TODO/vectors_2D.json
--rw-rw-rw-   0        0        0     2904 2022-07-11 12:10:26.615845 cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/1a_SAMPLING_TODO/vectors_3D.json
--rw-rw-rw-   0        0        0      444 2022-07-11 12:14:11.348217 cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/1b_SAMPLING_PENDING/clustering.json
--rw-rw-rw-   0        0        0        2 2022-07-11 12:10:27.067191 cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/1b_SAMPLING_PENDING/constraints.json
--rw-rw-rw-   0        0        0     1880 2022-08-23 13:18:42.002693 cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/1b_SAMPLING_PENDING/constraints_manager.pkl
--rw-rw-rw-   0        0        0      125 2022-07-11 12:27:05.724791 cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/1b_SAMPLING_PENDING/metadata.json
--rw-rw-rw-   0        0        0     3045 2022-07-11 12:10:27.509082 cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/1b_SAMPLING_PENDING/modelization.json
--rw-rw-rw-   0        0        0        2 2022-07-11 12:07:21.309471 cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/1b_SAMPLING_PENDING/sampling.json
--rw-rw-rw-   0        0        0     1580 2022-07-11 12:18:44.031863 cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/1b_SAMPLING_PENDING/settings.json
--rw-rw-rw-   0        0        0      174 2022-08-23 08:03:11.372441 cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/1b_SAMPLING_PENDING/status.json
--rw-rw-rw-   0        0        0     6513 2022-07-11 12:10:23.869094 cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/1b_SAMPLING_PENDING/texts.json
--rw-rw-rw-   0        0        0     5825 2022-07-11 12:10:24.327037 cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/1b_SAMPLING_PENDING/vectors.pkl
--rw-rw-rw-   0        0        0     2106 2022-07-11 12:10:25.284783 cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/1b_SAMPLING_PENDING/vectors_2D.json
--rw-rw-rw-   0        0        0     2904 2022-07-11 12:10:26.615845 cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/1b_SAMPLING_PENDING/vectors_3D.json
--rw-rw-rw-   0        0        0      444 2022-07-11 12:14:11.348217 cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/1c_SAMPLING_WORKING/clustering.json
--rw-rw-rw-   0        0        0        2 2022-07-11 12:10:27.067191 cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/1c_SAMPLING_WORKING/constraints.json
--rw-rw-rw-   0        0        0     1880 2022-08-23 13:18:42.008677 cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/1c_SAMPLING_WORKING/constraints_manager.pkl
--rw-rw-rw-   0        0        0      125 2022-07-11 12:27:12.700825 cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/1c_SAMPLING_WORKING/metadata.json
--rw-rw-rw-   0        0        0     3045 2022-07-11 12:10:27.509082 cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/1c_SAMPLING_WORKING/modelization.json
--rw-rw-rw-   0        0        0        2 2022-07-11 12:07:21.309471 cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/1c_SAMPLING_WORKING/sampling.json
--rw-rw-rw-   0        0        0     1580 2022-07-11 12:18:44.031863 cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/1c_SAMPLING_WORKING/settings.json
--rw-rw-rw-   0        0        0      167 2022-08-23 08:03:11.366457 cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/1c_SAMPLING_WORKING/status.json
--rw-rw-rw-   0        0        0     6513 2022-07-11 12:10:23.869094 cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/1c_SAMPLING_WORKING/texts.json
--rw-rw-rw-   0        0        0     5825 2022-07-11 12:10:24.327037 cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/1c_SAMPLING_WORKING/vectors.pkl
--rw-rw-rw-   0        0        0     2106 2022-07-11 12:10:25.284783 cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/1c_SAMPLING_WORKING/vectors_2D.json
--rw-rw-rw-   0        0        0     2904 2022-07-11 12:10:26.615845 cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/1c_SAMPLING_WORKING/vectors_3D.json
--rw-rw-rw-   0        0        0      444 2022-07-11 12:14:11.348217 cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/1d_ANNOTATION_WITH_UPTODATE_MODELIZATION/clustering.json
--rw-rw-rw-   0        0        0     9980 2022-07-11 12:20:33.453660 cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/1d_ANNOTATION_WITH_UPTODATE_MODELIZATION/constraints.json
--rw-rw-rw-   0        0        0     1880 2022-08-23 13:18:42.015672 cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/1d_ANNOTATION_WITH_UPTODATE_MODELIZATION/constraints_manager.pkl
--rw-rw-rw-   0        0        0      146 2022-07-11 12:27:29.714251 cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/1d_ANNOTATION_WITH_UPTODATE_MODELIZATION/metadata.json
--rw-rw-rw-   0        0        0     3045 2022-07-11 12:10:27.509082 cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/1d_ANNOTATION_WITH_UPTODATE_MODELIZATION/modelization.json
--rw-rw-rw-   0        0        0      498 2022-07-11 12:20:33.448671 cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/1d_ANNOTATION_WITH_UPTODATE_MODELIZATION/sampling.json
--rw-rw-rw-   0        0        0     1580 2022-07-11 12:18:44.031863 cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/1d_ANNOTATION_WITH_UPTODATE_MODELIZATION/settings.json
--rw-rw-rw-   0        0        0      101 2022-07-11 12:20:33.494108 cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/1d_ANNOTATION_WITH_UPTODATE_MODELIZATION/status.json
--rw-rw-rw-   0        0        0     6513 2022-07-11 12:10:23.869094 cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/1d_ANNOTATION_WITH_UPTODATE_MODELIZATION/texts.json
--rw-rw-rw-   0        0        0     5825 2022-07-11 12:10:24.327037 cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/1d_ANNOTATION_WITH_UPTODATE_MODELIZATION/vectors.pkl
--rw-rw-rw-   0        0        0     2106 2022-07-11 12:10:25.284783 cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/1d_ANNOTATION_WITH_UPTODATE_MODELIZATION/vectors_2D.json
--rw-rw-rw-   0        0        0     2904 2022-07-11 12:10:26.615845 cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/1d_ANNOTATION_WITH_UPTODATE_MODELIZATION/vectors_3D.json
--rw-rw-rw-   0        0        0      444 2022-07-11 12:14:11.348217 cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/1e_ANNOTATION_WITH_OUTDATED_MODELIZATION_WITHOUT_CONFLICTS/clustering.json
--rw-rw-rw-   0        0        0    11371 2022-07-11 13:20:21.670315 cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/1e_ANNOTATION_WITH_OUTDATED_MODELIZATION_WITHOUT_CONFLICTS/constraints.json
--rw-rw-rw-   0        0        0     2160 2022-08-23 13:18:42.021642 cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/1e_ANNOTATION_WITH_OUTDATED_MODELIZATION_WITHOUT_CONFLICTS/constraints_manager.pkl
--rw-rw-rw-   0        0        0      164 2022-07-11 13:26:02.683020 cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/1e_ANNOTATION_WITH_OUTDATED_MODELIZATION_WITHOUT_CONFLICTS/metadata.json
--rw-rw-rw-   0        0        0     3045 2022-07-11 13:21:08.841360 cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/1e_ANNOTATION_WITH_OUTDATED_MODELIZATION_WITHOUT_CONFLICTS/modelization.json
--rw-rw-rw-   0        0        0      498 2022-07-11 12:20:33.448671 cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/1e_ANNOTATION_WITH_OUTDATED_MODELIZATION_WITHOUT_CONFLICTS/sampling.json
--rw-rw-rw-   0        0        0     1580 2022-07-11 12:18:44.031863 cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/1e_ANNOTATION_WITH_OUTDATED_MODELIZATION_WITHOUT_CONFLICTS/settings.json
--rw-rw-rw-   0        0        0      119 2022-07-11 13:19:13.465236 cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/1e_ANNOTATION_WITH_OUTDATED_MODELIZATION_WITHOUT_CONFLICTS/status.json
--rw-rw-rw-   0        0        0     6512 2022-07-11 13:18:08.188828 cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/1e_ANNOTATION_WITH_OUTDATED_MODELIZATION_WITHOUT_CONFLICTS/texts.json
--rw-rw-rw-   0        0        0     5469 2022-07-11 13:18:08.637543 cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/1e_ANNOTATION_WITH_OUTDATED_MODELIZATION_WITHOUT_CONFLICTS/vectors.pkl
--rw-rw-rw-   0        0        0     2001 2022-07-11 13:18:09.816595 cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/1e_ANNOTATION_WITH_OUTDATED_MODELIZATION_WITHOUT_CONFLICTS/vectors_2D.json
--rw-rw-rw-   0        0        0     2773 2022-07-11 13:18:10.735536 cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/1e_ANNOTATION_WITH_OUTDATED_MODELIZATION_WITHOUT_CONFLICTS/vectors_3D.json
--rw-rw-rw-   0        0        0      444 2022-07-11 12:14:11.348217 cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/1f_ANNOTATION_WITH_PENDING_MODELIZATION_WITHOUT_CONFLICTS/clustering.json
--rw-rw-rw-   0        0        0    11371 2022-07-11 13:20:21.670315 cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/1f_ANNOTATION_WITH_PENDING_MODELIZATION_WITHOUT_CONFLICTS/constraints.json
--rw-rw-rw-   0        0        0     2160 2022-08-23 13:18:42.028634 cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/1f_ANNOTATION_WITH_PENDING_MODELIZATION_WITHOUT_CONFLICTS/constraints_manager.pkl
--rw-rw-rw-   0        0        0      163 2022-07-11 13:24:30.805153 cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/1f_ANNOTATION_WITH_PENDING_MODELIZATION_WITHOUT_CONFLICTS/metadata.json
--rw-rw-rw-   0        0        0     3045 2022-07-11 13:21:08.841360 cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/1f_ANNOTATION_WITH_PENDING_MODELIZATION_WITHOUT_CONFLICTS/modelization.json
--rw-rw-rw-   0        0        0      498 2022-07-11 12:20:33.448671 cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/1f_ANNOTATION_WITH_PENDING_MODELIZATION_WITHOUT_CONFLICTS/sampling.json
--rw-rw-rw-   0        0        0     1580 2022-07-11 12:18:44.031863 cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/1f_ANNOTATION_WITH_PENDING_MODELIZATION_WITHOUT_CONFLICTS/settings.json
--rw-rw-rw-   0        0        0      212 2022-08-23 08:03:11.366457 cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/1f_ANNOTATION_WITH_PENDING_MODELIZATION_WITHOUT_CONFLICTS/status.json
--rw-rw-rw-   0        0        0     6512 2022-07-11 13:18:08.188828 cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/1f_ANNOTATION_WITH_PENDING_MODELIZATION_WITHOUT_CONFLICTS/texts.json
--rw-rw-rw-   0        0        0     5469 2022-07-11 13:18:08.637543 cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/1f_ANNOTATION_WITH_PENDING_MODELIZATION_WITHOUT_CONFLICTS/vectors.pkl
--rw-rw-rw-   0        0        0     2001 2022-07-11 13:18:09.816595 cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/1f_ANNOTATION_WITH_PENDING_MODELIZATION_WITHOUT_CONFLICTS/vectors_2D.json
--rw-rw-rw-   0        0        0     2773 2022-07-11 13:18:10.735536 cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/1f_ANNOTATION_WITH_PENDING_MODELIZATION_WITHOUT_CONFLICTS/vectors_3D.json
--rw-rw-rw-   0        0        0      444 2022-07-11 12:14:11.348217 cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/1g_ANNOTATION_WITH_WORKING_MODELIZATION_WITHOUT_CONFLICTS/clustering.json
--rw-rw-rw-   0        0        0    11371 2022-07-11 13:20:21.670315 cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/1g_ANNOTATION_WITH_WORKING_MODELIZATION_WITHOUT_CONFLICTS/constraints.json
--rw-rw-rw-   0        0        0     2160 2022-08-23 13:18:42.035605 cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/1g_ANNOTATION_WITH_WORKING_MODELIZATION_WITHOUT_CONFLICTS/constraints_manager.pkl
--rw-rw-rw-   0        0        0      163 2022-07-11 13:23:55.651507 cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/1g_ANNOTATION_WITH_WORKING_MODELIZATION_WITHOUT_CONFLICTS/metadata.json
--rw-rw-rw-   0        0        0     3045 2022-07-11 13:21:08.841360 cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/1g_ANNOTATION_WITH_WORKING_MODELIZATION_WITHOUT_CONFLICTS/modelization.json
--rw-rw-rw-   0        0        0      498 2022-07-11 12:20:33.448671 cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/1g_ANNOTATION_WITH_WORKING_MODELIZATION_WITHOUT_CONFLICTS/sampling.json
--rw-rw-rw-   0        0        0     1580 2022-07-11 12:18:44.031863 cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/1g_ANNOTATION_WITH_WORKING_MODELIZATION_WITHOUT_CONFLICTS/settings.json
--rw-rw-rw-   0        0        0      189 2022-08-23 08:03:11.362489 cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/1g_ANNOTATION_WITH_WORKING_MODELIZATION_WITHOUT_CONFLICTS/status.json
--rw-rw-rw-   0        0        0     6512 2022-07-11 13:18:08.188828 cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/1g_ANNOTATION_WITH_WORKING_MODELIZATION_WITHOUT_CONFLICTS/texts.json
--rw-rw-rw-   0        0        0     5469 2022-07-11 13:18:08.637543 cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/1g_ANNOTATION_WITH_WORKING_MODELIZATION_WITHOUT_CONFLICTS/vectors.pkl
--rw-rw-rw-   0        0        0     2001 2022-07-11 13:18:09.816595 cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/1g_ANNOTATION_WITH_WORKING_MODELIZATION_WITHOUT_CONFLICTS/vectors_2D.json
--rw-rw-rw-   0        0        0     2773 2022-07-11 13:18:10.735536 cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/1g_ANNOTATION_WITH_WORKING_MODELIZATION_WITHOUT_CONFLICTS/vectors_3D.json
--rw-rw-rw-   0        0        0      444 2022-07-11 12:14:11.348217 cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/1h_ANNOTATION_WITH_OUTDATED_MODELIZATION_WITH_CONFLICTS/clustering.json
--rw-rw-rw-   0        0        0    11370 2022-07-11 13:21:59.471239 cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/1h_ANNOTATION_WITH_OUTDATED_MODELIZATION_WITH_CONFLICTS/constraints.json
--rw-rw-rw-   0        0        0     2169 2022-08-23 13:18:42.042584 cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/1h_ANNOTATION_WITH_OUTDATED_MODELIZATION_WITH_CONFLICTS/constraints_manager.pkl
--rw-rw-rw-   0        0        0      161 2022-07-11 13:23:30.838275 cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/1h_ANNOTATION_WITH_OUTDATED_MODELIZATION_WITH_CONFLICTS/metadata.json
--rw-rw-rw-   0        0        0     7327 2022-07-11 13:21:59.906137 cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/1h_ANNOTATION_WITH_OUTDATED_MODELIZATION_WITH_CONFLICTS/modelization.json
--rw-rw-rw-   0        0        0      498 2022-07-11 12:20:33.448671 cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/1h_ANNOTATION_WITH_OUTDATED_MODELIZATION_WITH_CONFLICTS/sampling.json
--rw-rw-rw-   0        0        0     1580 2022-07-11 12:18:44.031863 cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/1h_ANNOTATION_WITH_OUTDATED_MODELIZATION_WITH_CONFLICTS/settings.json
--rw-rw-rw-   0        0        0      116 2022-07-11 13:21:59.916111 cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/1h_ANNOTATION_WITH_OUTDATED_MODELIZATION_WITH_CONFLICTS/status.json
--rw-rw-rw-   0        0        0     6512 2022-07-11 13:21:55.273853 cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/1h_ANNOTATION_WITH_OUTDATED_MODELIZATION_WITH_CONFLICTS/texts.json
--rw-rw-rw-   0        0        0     5469 2022-07-11 13:21:55.838885 cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/1h_ANNOTATION_WITH_OUTDATED_MODELIZATION_WITH_CONFLICTS/vectors.pkl
--rw-rw-rw-   0        0        0     2001 2022-07-11 13:21:57.677538 cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/1h_ANNOTATION_WITH_OUTDATED_MODELIZATION_WITH_CONFLICTS/vectors_2D.json
--rw-rw-rw-   0        0        0     2773 2022-07-11 13:21:59.020204 cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/1h_ANNOTATION_WITH_OUTDATED_MODELIZATION_WITH_CONFLICTS/vectors_3D.json
--rw-rw-rw-   0        0        0      444 2022-07-11 12:14:11.348217 cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/1i_ANNOTATION_WITH_OUTDATED_MODELIZATION_WITH_CONFLICTS/clustering.json
--rw-rw-rw-   0        0        0    11443 2022-07-11 13:30:14.546184 cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/1i_ANNOTATION_WITH_OUTDATED_MODELIZATION_WITH_CONFLICTS/constraints.json
--rw-rw-rw-   0        0        0     2169 2022-08-23 13:18:42.048571 cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/1i_ANNOTATION_WITH_OUTDATED_MODELIZATION_WITH_CONFLICTS/constraints_manager.pkl
--rw-rw-rw-   0        0        0      161 2022-07-11 13:28:17.222075 cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/1i_ANNOTATION_WITH_OUTDATED_MODELIZATION_WITH_CONFLICTS/metadata.json
--rw-rw-rw-   0        0        0     7327 2022-07-11 13:29:05.933834 cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/1i_ANNOTATION_WITH_OUTDATED_MODELIZATION_WITH_CONFLICTS/modelization.json
--rw-rw-rw-   0        0        0      498 2022-07-11 12:20:33.448671 cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/1i_ANNOTATION_WITH_OUTDATED_MODELIZATION_WITH_CONFLICTS/sampling.json
--rw-rw-rw-   0        0        0     1580 2022-07-11 12:18:44.031863 cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/1i_ANNOTATION_WITH_OUTDATED_MODELIZATION_WITH_CONFLICTS/settings.json
--rw-rw-rw-   0        0        0      116 2022-07-11 13:30:14.540199 cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/1i_ANNOTATION_WITH_OUTDATED_MODELIZATION_WITH_CONFLICTS/status.json
--rw-rw-rw-   0        0        0     6512 2022-07-11 13:29:02.736926 cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/1i_ANNOTATION_WITH_OUTDATED_MODELIZATION_WITH_CONFLICTS/texts.json
--rw-rw-rw-   0        0        0     5469 2022-07-11 13:29:03.209019 cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/1i_ANNOTATION_WITH_OUTDATED_MODELIZATION_WITH_CONFLICTS/vectors.pkl
--rw-rw-rw-   0        0        0     2001 2022-07-11 13:29:04.093840 cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/1i_ANNOTATION_WITH_OUTDATED_MODELIZATION_WITH_CONFLICTS/vectors_2D.json
--rw-rw-rw-   0        0        0     2773 2022-07-11 13:29:05.015142 cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/1i_ANNOTATION_WITH_OUTDATED_MODELIZATION_WITH_CONFLICTS/vectors_3D.json
--rw-rw-rw-   0        0        0      444 2022-07-11 12:14:11.348217 cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/1j_ANNOTATION_WITH_PENDING_MODELIZATION_WITH_CONFLICTS/clustering.json
--rw-rw-rw-   0        0        0    11443 2022-07-11 13:30:14.546184 cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/1j_ANNOTATION_WITH_PENDING_MODELIZATION_WITH_CONFLICTS/constraints.json
--rw-rw-rw-   0        0        0     2169 2022-08-23 13:18:42.054553 cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/1j_ANNOTATION_WITH_PENDING_MODELIZATION_WITH_CONFLICTS/constraints_manager.pkl
--rw-rw-rw-   0        0        0      160 2022-07-11 13:33:48.143189 cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/1j_ANNOTATION_WITH_PENDING_MODELIZATION_WITH_CONFLICTS/metadata.json
--rw-rw-rw-   0        0        0     7327 2022-07-11 13:29:05.933834 cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/1j_ANNOTATION_WITH_PENDING_MODELIZATION_WITH_CONFLICTS/modelization.json
--rw-rw-rw-   0        0        0      498 2022-07-11 12:20:33.448671 cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/1j_ANNOTATION_WITH_PENDING_MODELIZATION_WITH_CONFLICTS/sampling.json
--rw-rw-rw-   0        0        0     1580 2022-07-11 12:18:44.031863 cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/1j_ANNOTATION_WITH_PENDING_MODELIZATION_WITH_CONFLICTS/settings.json
--rw-rw-rw-   0        0        0      209 2022-08-23 08:03:11.358480 cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/1j_ANNOTATION_WITH_PENDING_MODELIZATION_WITH_CONFLICTS/status.json
--rw-rw-rw-   0        0        0     6512 2022-07-11 13:29:02.736926 cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/1j_ANNOTATION_WITH_PENDING_MODELIZATION_WITH_CONFLICTS/texts.json
--rw-rw-rw-   0        0        0     5469 2022-07-11 13:29:03.209019 cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/1j_ANNOTATION_WITH_PENDING_MODELIZATION_WITH_CONFLICTS/vectors.pkl
--rw-rw-rw-   0        0        0     2001 2022-07-11 13:29:04.093840 cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/1j_ANNOTATION_WITH_PENDING_MODELIZATION_WITH_CONFLICTS/vectors_2D.json
--rw-rw-rw-   0        0        0     2773 2022-07-11 13:29:05.015142 cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/1j_ANNOTATION_WITH_PENDING_MODELIZATION_WITH_CONFLICTS/vectors_3D.json
--rw-rw-rw-   0        0        0      444 2022-07-11 12:14:11.348217 cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/1k_ANNOTATION_WITH_WORKING_MODELIZATION_WITH_CONFLICTS/clustering.json
--rw-rw-rw-   0        0        0    11443 2022-07-11 13:30:14.546184 cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/1k_ANNOTATION_WITH_WORKING_MODELIZATION_WITH_CONFLICTS/constraints.json
--rw-rw-rw-   0        0        0     2169 2022-08-23 13:18:42.061533 cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/1k_ANNOTATION_WITH_WORKING_MODELIZATION_WITH_CONFLICTS/constraints_manager.pkl
--rw-rw-rw-   0        0        0      160 2022-07-11 13:32:51.404211 cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/1k_ANNOTATION_WITH_WORKING_MODELIZATION_WITH_CONFLICTS/metadata.json
--rw-rw-rw-   0        0        0     7327 2022-07-11 13:29:05.933834 cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/1k_ANNOTATION_WITH_WORKING_MODELIZATION_WITH_CONFLICTS/modelization.json
--rw-rw-rw-   0        0        0      498 2022-07-11 12:20:33.448671 cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/1k_ANNOTATION_WITH_WORKING_MODELIZATION_WITH_CONFLICTS/sampling.json
--rw-rw-rw-   0        0        0     1580 2022-07-11 12:18:44.031863 cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/1k_ANNOTATION_WITH_WORKING_MODELIZATION_WITH_CONFLICTS/settings.json
--rw-rw-rw-   0        0        0      186 2022-08-23 08:03:11.358480 cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/1k_ANNOTATION_WITH_WORKING_MODELIZATION_WITH_CONFLICTS/status.json
--rw-rw-rw-   0        0        0     6512 2022-07-11 13:29:02.736926 cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/1k_ANNOTATION_WITH_WORKING_MODELIZATION_WITH_CONFLICTS/texts.json
--rw-rw-rw-   0        0        0     5469 2022-07-11 13:29:03.209019 cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/1k_ANNOTATION_WITH_WORKING_MODELIZATION_WITH_CONFLICTS/vectors.pkl
--rw-rw-rw-   0        0        0     2001 2022-07-11 13:29:04.093840 cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/1k_ANNOTATION_WITH_WORKING_MODELIZATION_WITH_CONFLICTS/vectors_2D.json
--rw-rw-rw-   0        0        0     2773 2022-07-11 13:29:05.015142 cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/1k_ANNOTATION_WITH_WORKING_MODELIZATION_WITH_CONFLICTS/vectors_3D.json
--rw-rw-rw-   0        0        0      444 2022-07-11 12:14:11.348217 cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/1l_ANNOTATION_WITH_UPTODATE_MODELIZATION/clustering.json
--rw-rw-rw-   0        0        0    11444 2022-07-11 13:32:13.084020 cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/1l_ANNOTATION_WITH_UPTODATE_MODELIZATION/constraints.json
--rw-rw-rw-   0        0        0     2160 2022-08-23 13:18:42.067517 cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/1l_ANNOTATION_WITH_UPTODATE_MODELIZATION/constraints_manager.pkl
--rw-rw-rw-   0        0        0      146 2022-07-11 13:35:34.340671 cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/1l_ANNOTATION_WITH_UPTODATE_MODELIZATION/metadata.json
--rw-rw-rw-   0        0        0     7549 2022-07-11 13:32:13.556194 cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/1l_ANNOTATION_WITH_UPTODATE_MODELIZATION/modelization.json
--rw-rw-rw-   0        0        0      498 2022-07-11 12:20:33.448671 cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/1l_ANNOTATION_WITH_UPTODATE_MODELIZATION/sampling.json
--rw-rw-rw-   0        0        0     1580 2022-07-11 12:18:44.031863 cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/1l_ANNOTATION_WITH_UPTODATE_MODELIZATION/settings.json
--rw-rw-rw-   0        0        0      101 2022-07-11 13:32:13.567680 cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/1l_ANNOTATION_WITH_UPTODATE_MODELIZATION/status.json
--rw-rw-rw-   0        0        0     6512 2022-07-11 13:32:09.435685 cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/1l_ANNOTATION_WITH_UPTODATE_MODELIZATION/texts.json
--rw-rw-rw-   0        0        0     5469 2022-07-11 13:32:09.842201 cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/1l_ANNOTATION_WITH_UPTODATE_MODELIZATION/vectors.pkl
--rw-rw-rw-   0        0        0     2001 2022-07-11 13:32:11.354109 cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/1l_ANNOTATION_WITH_UPTODATE_MODELIZATION/vectors_2D.json
--rw-rw-rw-   0        0        0     2773 2022-07-11 13:32:12.581956 cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/1l_ANNOTATION_WITH_UPTODATE_MODELIZATION/vectors_3D.json
--rw-rw-rw-   0        0        0      444 2022-07-11 12:14:11.348217 cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/1m_CLUSTERING_TODO/clustering.json
--rw-rw-rw-   0        0        0    11444 2022-07-11 13:32:13.084020 cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/1m_CLUSTERING_TODO/constraints.json
--rw-rw-rw-   0        0        0     2160 2022-08-23 13:18:42.073502 cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/1m_CLUSTERING_TODO/constraints_manager.pkl
--rw-rw-rw-   0        0        0      124 2022-07-11 13:36:31.126577 cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/1m_CLUSTERING_TODO/metadata.json
--rw-rw-rw-   0        0        0     7549 2022-07-11 13:32:13.556194 cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/1m_CLUSTERING_TODO/modelization.json
--rw-rw-rw-   0        0        0      498 2022-07-11 12:20:33.448671 cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/1m_CLUSTERING_TODO/sampling.json
--rw-rw-rw-   0        0        0     1580 2022-07-11 12:18:44.031863 cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/1m_CLUSTERING_TODO/settings.json
--rw-rw-rw-   0        0        0       79 2022-07-11 13:35:55.828058 cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/1m_CLUSTERING_TODO/status.json
--rw-rw-rw-   0        0        0     6512 2022-07-11 13:32:09.435685 cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/1m_CLUSTERING_TODO/texts.json
--rw-rw-rw-   0        0        0     5469 2022-07-11 13:32:09.842201 cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/1m_CLUSTERING_TODO/vectors.pkl
--rw-rw-rw-   0        0        0     2001 2022-07-11 13:32:11.354109 cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/1m_CLUSTERING_TODO/vectors_2D.json
--rw-rw-rw-   0        0        0     2773 2022-07-11 13:32:12.581956 cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/1m_CLUSTERING_TODO/vectors_3D.json
--rw-rw-rw-   0        0        0      444 2022-07-11 12:14:11.348217 cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/1n_CLUSTERING_PENDING/clustering.json
--rw-rw-rw-   0        0        0    11444 2022-07-11 13:32:13.084020 cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/1n_CLUSTERING_PENDING/constraints.json
--rw-rw-rw-   0        0        0     2160 2022-08-23 13:18:42.080483 cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/1n_CLUSTERING_PENDING/constraints_manager.pkl
--rw-rw-rw-   0        0        0      127 2022-07-11 13:38:11.134105 cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/1n_CLUSTERING_PENDING/metadata.json
--rw-rw-rw-   0        0        0     7549 2022-07-11 13:32:13.556194 cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/1n_CLUSTERING_PENDING/modelization.json
--rw-rw-rw-   0        0        0      498 2022-07-11 12:20:33.448671 cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/1n_CLUSTERING_PENDING/sampling.json
--rw-rw-rw-   0        0        0     1580 2022-07-11 12:18:44.031863 cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/1n_CLUSTERING_PENDING/settings.json
--rw-rw-rw-   0        0        0      176 2022-08-23 08:03:11.358480 cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/1n_CLUSTERING_PENDING/status.json
--rw-rw-rw-   0        0        0     6512 2022-07-11 13:32:09.435685 cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/1n_CLUSTERING_PENDING/texts.json
--rw-rw-rw-   0        0        0     5469 2022-07-11 13:32:09.842201 cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/1n_CLUSTERING_PENDING/vectors.pkl
--rw-rw-rw-   0        0        0     2001 2022-07-11 13:32:11.354109 cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/1n_CLUSTERING_PENDING/vectors_2D.json
--rw-rw-rw-   0        0        0     2773 2022-07-11 13:32:12.581956 cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/1n_CLUSTERING_PENDING/vectors_3D.json
--rw-rw-rw-   0        0        0      444 2022-07-11 12:14:11.348217 cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/1o_CLUSTERING_WORKING/clustering.json
--rw-rw-rw-   0        0        0    11444 2022-07-11 13:32:13.084020 cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/1o_CLUSTERING_WORKING/constraints.json
--rw-rw-rw-   0        0        0     2160 2022-08-23 13:18:42.086467 cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/1o_CLUSTERING_WORKING/constraints_manager.pkl
--rw-rw-rw-   0        0        0      127 2022-07-11 13:38:57.822291 cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/1o_CLUSTERING_WORKING/metadata.json
--rw-rw-rw-   0        0        0     7549 2022-07-11 13:32:13.556194 cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/1o_CLUSTERING_WORKING/modelization.json
--rw-rw-rw-   0        0        0      498 2022-07-11 12:20:33.448671 cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/1o_CLUSTERING_WORKING/sampling.json
--rw-rw-rw-   0        0        0     1580 2022-07-11 12:18:44.031863 cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/1o_CLUSTERING_WORKING/settings.json
--rw-rw-rw-   0        0        0      163 2022-08-23 08:03:11.356483 cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/1o_CLUSTERING_WORKING/status.json
--rw-rw-rw-   0        0        0     6512 2022-07-11 13:32:09.435685 cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/1o_CLUSTERING_WORKING/texts.json
--rw-rw-rw-   0        0        0     5469 2022-07-11 13:32:09.842201 cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/1o_CLUSTERING_WORKING/vectors.pkl
--rw-rw-rw-   0        0        0     2001 2022-07-11 13:32:11.354109 cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/1o_CLUSTERING_WORKING/vectors_2D.json
--rw-rw-rw-   0        0        0     2773 2022-07-11 13:32:12.581956 cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/1o_CLUSTERING_WORKING/vectors_3D.json
--rw-rw-rw-   0        0        0      867 2022-07-11 13:37:45.568647 cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/1p_ITERATION_END/clustering.json
--rw-rw-rw-   0        0        0    11444 2022-07-11 13:32:13.084020 cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/1p_ITERATION_END/constraints.json
--rw-rw-rw-   0        0        0     2160 2022-08-23 13:18:42.092451 cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/1p_ITERATION_END/constraints_manager.pkl
--rw-rw-rw-   0        0        0      122 2022-07-11 13:40:36.003123 cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/1p_ITERATION_END/metadata.json
--rw-rw-rw-   0        0        0     7549 2022-07-11 13:32:13.556194 cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/1p_ITERATION_END/modelization.json
--rw-rw-rw-   0        0        0      498 2022-07-11 12:20:33.448671 cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/1p_ITERATION_END/sampling.json
--rw-rw-rw-   0        0        0     1580 2022-07-11 12:18:44.031863 cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/1p_ITERATION_END/settings.json
--rw-rw-rw-   0        0        0       77 2022-07-11 13:37:45.590987 cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/1p_ITERATION_END/status.json
--rw-rw-rw-   0        0        0     6512 2022-07-11 13:32:09.435685 cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/1p_ITERATION_END/texts.json
--rw-rw-rw-   0        0        0     5469 2022-07-11 13:32:09.842201 cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/1p_ITERATION_END/vectors.pkl
--rw-rw-rw-   0        0        0     2001 2022-07-11 13:32:11.354109 cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/1p_ITERATION_END/vectors_2D.json
--rw-rw-rw-   0        0        0     2773 2022-07-11 13:32:12.581956 cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/1p_ITERATION_END/vectors_3D.json
--rw-rw-rw-   0        0        0      867 2022-07-11 13:37:45.568647 cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/2a_SAMPLING_TODO/clustering.json
--rw-rw-rw-   0        0        0    11444 2022-07-11 13:32:13.084020 cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/2a_SAMPLING_TODO/constraints.json
--rw-rw-rw-   0        0        0     2160 2022-08-23 13:18:42.099434 cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/2a_SAMPLING_TODO/constraints_manager.pkl
--rw-rw-rw-   0        0        0      122 2022-07-11 13:40:36.003123 cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/2a_SAMPLING_TODO/metadata.json
--rw-rw-rw-   0        0        0     7549 2022-07-11 13:32:13.556194 cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/2a_SAMPLING_TODO/modelization.json
--rw-rw-rw-   0        0        0      498 2022-07-11 12:20:33.448671 cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/2a_SAMPLING_TODO/sampling.json
--rw-rw-rw-   0        0        0     2627 2022-08-16 13:06:28.980097 cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/2a_SAMPLING_TODO/settings.json
--rw-rw-rw-   0        0        0       77 2022-07-26 08:52:16.772181 cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/2a_SAMPLING_TODO/status.json
--rw-rw-rw-   0        0        0     6512 2022-07-11 13:32:09.435685 cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/2a_SAMPLING_TODO/texts.json
--rw-rw-rw-   0        0        0     5469 2022-07-11 13:32:09.842201 cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/2a_SAMPLING_TODO/vectors.pkl
--rw-rw-rw-   0        0        0     2001 2022-07-11 13:32:11.354109 cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/2a_SAMPLING_TODO/vectors_2D.json
--rw-rw-rw-   0        0        0     2773 2022-07-11 13:32:12.581956 cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/2a_SAMPLING_TODO/vectors_3D.json
--rw-rw-rw-   0        0        0      885 2022-08-16 13:41:53.919265 cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/2b2_SAMPLING_PENDING/clustering.json
--rw-rw-rw-   0        0        0     9980 2022-07-11 12:20:33.453660 cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/2b2_SAMPLING_PENDING/constraints.json
--rw-rw-rw-   0        0        0     1880 2022-08-23 13:18:42.105416 cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/2b2_SAMPLING_PENDING/constraints_manager.pkl
--rw-rw-rw-   0        0        0      122 2022-07-11 13:40:36.003123 cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/2b2_SAMPLING_PENDING/metadata.json
--rw-rw-rw-   0        0        0     7549 2022-07-11 13:32:13.556194 cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/2b2_SAMPLING_PENDING/modelization.json
--rw-rw-rw-   0        0        0      498 2022-08-18 10:46:51.121529 cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/2b2_SAMPLING_PENDING/sampling.json
--rw-rw-rw-   0        0        0     2627 2022-08-16 13:06:04.636697 cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/2b2_SAMPLING_PENDING/settings.json
--rw-rw-rw-   0        0        0      175 2022-08-23 08:03:11.350499 cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/2b2_SAMPLING_PENDING/status.json
--rw-rw-rw-   0        0        0     6513 2022-08-16 13:42:08.834581 cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/2b2_SAMPLING_PENDING/texts.json
--rw-rw-rw-   0        0        0     5825 2022-07-11 12:10:24.327037 cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/2b2_SAMPLING_PENDING/vectors.pkl
--rw-rw-rw-   0        0        0     2106 2022-07-11 12:10:25.284783 cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/2b2_SAMPLING_PENDING/vectors_2D.json
--rw-rw-rw-   0        0        0     2904 2022-07-11 12:10:26.615845 cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/2b2_SAMPLING_PENDING/vectors_3D.json
--rw-rw-rw-   0        0        0      867 2022-07-11 13:37:45.568647 cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/2b_SAMPLING_PENDING/clustering.json
--rw-rw-rw-   0        0        0    11444 2022-07-11 13:32:13.084020 cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/2b_SAMPLING_PENDING/constraints.json
--rw-rw-rw-   0        0        0     2160 2022-08-23 13:18:42.111400 cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/2b_SAMPLING_PENDING/constraints_manager.pkl
--rw-rw-rw-   0        0        0      122 2022-07-11 13:40:36.003123 cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/2b_SAMPLING_PENDING/metadata.json
--rw-rw-rw-   0        0        0     7549 2022-07-11 13:32:13.556194 cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/2b_SAMPLING_PENDING/modelization.json
--rw-rw-rw-   0        0        0      498 2022-07-11 12:20:33.448671 cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/2b_SAMPLING_PENDING/sampling.json
--rw-rw-rw-   0        0        0     2627 2022-08-16 13:06:04.636697 cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/2b_SAMPLING_PENDING/settings.json
--rw-rw-rw-   0        0        0      175 2022-08-23 08:03:11.351497 cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/2b_SAMPLING_PENDING/status.json
--rw-rw-rw-   0        0        0     6512 2022-07-11 13:32:09.435685 cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/2b_SAMPLING_PENDING/texts.json
--rw-rw-rw-   0        0        0     5469 2022-07-11 13:32:09.842201 cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/2b_SAMPLING_PENDING/vectors.pkl
--rw-rw-rw-   0        0        0     2001 2022-07-11 13:32:11.354109 cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/2b_SAMPLING_PENDING/vectors_2D.json
--rw-rw-rw-   0        0        0     2773 2022-07-11 13:32:12.581956 cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/2b_SAMPLING_PENDING/vectors_3D.json
--rw-rw-rw-   0        0        0      867 2022-07-11 13:37:45.568647 cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/2d_ANNOTATION_WITH_UPTODATE_MODELIZATION/clustering.json
--rw-rw-rw-   0        0        0    64545 2022-08-16 13:19:03.162721 cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/2d_ANNOTATION_WITH_UPTODATE_MODELIZATION/constraints.json
--rw-rw-rw-   0        0        0     2160 2022-08-23 13:18:42.118384 cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/2d_ANNOTATION_WITH_UPTODATE_MODELIZATION/constraints_manager.pkl
--rw-rw-rw-   0        0        0      146 2022-07-11 13:45:33.025114 cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/2d_ANNOTATION_WITH_UPTODATE_MODELIZATION/metadata.json
--rw-rw-rw-   0        0        0     7549 2022-07-11 13:32:13.556194 cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/2d_ANNOTATION_WITH_UPTODATE_MODELIZATION/modelization.json
--rw-rw-rw-   0        0        0     5807 2022-08-18 10:46:39.012624 cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/2d_ANNOTATION_WITH_UPTODATE_MODELIZATION/sampling.json
--rw-rw-rw-   0        0        0     2627 2022-08-16 13:06:18.718616 cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/2d_ANNOTATION_WITH_UPTODATE_MODELIZATION/settings.json
--rw-rw-rw-   0        0        0      101 2022-07-11 13:45:09.965237 cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/2d_ANNOTATION_WITH_UPTODATE_MODELIZATION/status.json
--rw-rw-rw-   0        0        0     6512 2022-07-11 13:32:09.435685 cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/2d_ANNOTATION_WITH_UPTODATE_MODELIZATION/texts.json
--rw-rw-rw-   0        0        0     5469 2022-07-11 13:32:09.842201 cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/2d_ANNOTATION_WITH_UPTODATE_MODELIZATION/vectors.pkl
--rw-rw-rw-   0        0        0     2001 2022-07-11 13:32:11.354109 cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/2d_ANNOTATION_WITH_UPTODATE_MODELIZATION/vectors_2D.json
--rw-rw-rw-   0        0        0     2773 2022-07-11 13:32:12.581956 cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/2d_ANNOTATION_WITH_UPTODATE_MODELIZATION/vectors_3D.json
--rw-rw-rw-   0        0        0     2443 2022-07-19 13:23:52.519541 cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/archive-0a_INITIALIZATION_WITHOUT_MODELIZATION.zip
--rw-rw-rw-   0        0        0     4445 2022-07-11 14:10:29.043689 cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/archive-1b_SAMPLING_PENDING.zip
--rw-rw-rw-   0        0        0     4930 2022-07-11 14:00:42.949467 cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/archive-1d_ANNOTATION_WITH_UPTODATE_MODELIZATION.zip
--rw-rw-rw-   0        0        0     5368 2022-07-21 13:33:48.984320 cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/archive-1h_ANNOTATION_WITH_OUTDATED_MODELIZATION_WITH_CONFLICTS.zip
--rw-rw-rw-   0        0        0     5422 2022-07-11 14:11:07.712387 cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/archive-1j_ANNOTATION_WITH_PENDING_MODELIZATION_WITH_CONFLICTS.zip
--rw-rw-rw-   0        0        0     5367 2022-07-20 08:54:04.397687 cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/archive-1l_ANNOTATION_WITH_UPTODATE_MODELIZATION.zip
--rw-rw-rw-   0        0        0    11846 2022-07-19 13:18:15.405915 cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/archive-1o_CLUSTERING_WORKING.zip
--rw-rw-rw-   0        0        0     8324 2022-07-19 13:18:57.703046 cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/archive-1p_ITERATION_END.zip
--rw-rw-rw-   0        0        0     3361 2022-07-19 13:52:29.115912 cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/archive-ERROR_bad_archive.zip
--rw-rw-rw-   0        0        0     4439 2022-07-19 13:18:34.810168 cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/archive-ERROR_metadata_bad_creation_timestamp.zip
--rw-rw-rw-   0        0        0     4450 2022-07-19 13:18:53.508055 cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/archive-ERROR_metadata_bad_project_name.zip
--rw-rw-rw-   0        0        0     4415 2022-07-19 13:19:23.354348 cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/archive-ERROR_metadata_missing_creation_timestamp.zip
--rw-rw-rw-   0        0        0     4424 2022-07-19 13:19:38.863582 cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/archive-ERROR_metadata_missing_project_name.zip
--rw-rw-rw-   0        0        0     1185 2022-07-19 13:31:51.308161 cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/archive-ERROR_missing_files.zip
--rw-rw-rw-   0        0        0     4428 2022-07-19 13:20:13.283333 cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/archive-ERROR_status_bad_state.zip
--rw-rw-rw-   0        0        0     4409 2022-07-19 13:20:35.454944 cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/archive-ERROR_status_missing_state.zip
--rw-rw-rw-   0        0        0     1098 2022-07-12 15:28:00.547593 cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/dummy_24.csv
--rw-rw-rw-   0        0        0     1075 2022-07-12 14:12:39.131119 cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/dummy_24.txt
--rw-rw-rw-   0        0        0     9095 2022-07-11 11:58:18.587515 cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/dummy_24.xlsx
--rw-rw-rw-   0        0        0     1110 2022-07-11 11:57:06.067159 cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/dummy_24_err.csv
--rw-rw-rw-   0        0        0     9122 2022-07-11 11:58:06.501182 cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/dummy_24_err.xlsx
--rw-rw-rw-   0        0        0        2 2022-07-11 12:07:21.312463 cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/import_0y0_INITIALIZATION_WITHOUT_MODELIZATION/clustering.json
--rw-rw-rw-   0        0        0        2 2022-07-11 12:07:21.271572 cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/import_0y0_INITIALIZATION_WITHOUT_MODELIZATION/constraints.json
--rw-rw-rw-   0        0        0      152 2022-07-29 10:04:12.529088 cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/import_0y0_INITIALIZATION_WITHOUT_MODELIZATION/metadata.json
--rw-rw-rw-   0        0        0     3045 2022-07-11 12:07:21.303486 cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/import_0y0_INITIALIZATION_WITHOUT_MODELIZATION/modelization.json
--rw-rw-rw-   0        0        0        2 2022-07-11 12:07:21.309471 cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/import_0y0_INITIALIZATION_WITHOUT_MODELIZATION/sampling.json
--rw-rw-rw-   0        0        0      696 2022-07-11 12:13:45.311609 cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/import_0y0_INITIALIZATION_WITHOUT_MODELIZATION/settings.json
--rw-rw-rw-   0        0        0       99 2022-07-11 12:07:21.264592 cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/import_0y0_INITIALIZATION_WITHOUT_MODELIZATION/status.json
--rw-rw-rw-   0        0        0     6659 2022-07-11 12:07:21.267583 cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/import_0y0_INITIALIZATION_WITHOUT_MODELIZATION/texts.json
--rw-rw-rw-   0        0        0        2 2022-07-11 12:07:21.312463 cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/import_0y1_INITIALIZATION_WITH_PENDING_MODELIZATION/clustering.json
--rw-rw-rw-   0        0        0        2 2022-07-11 12:07:21.271572 cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/import_0y1_INITIALIZATION_WITH_PENDING_MODELIZATION/constraints.json
--rw-rw-rw-   0        0        0      157 2022-07-29 10:04:49.540024 cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/import_0y1_INITIALIZATION_WITH_PENDING_MODELIZATION/metadata.json
--rw-rw-rw-   0        0        0     3045 2022-07-11 12:07:21.303486 cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/import_0y1_INITIALIZATION_WITH_PENDING_MODELIZATION/modelization.json
--rw-rw-rw-   0        0        0        2 2022-07-11 12:07:21.309471 cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/import_0y1_INITIALIZATION_WITH_PENDING_MODELIZATION/sampling.json
--rw-rw-rw-   0        0        0      696 2022-07-11 12:13:45.311609 cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/import_0y1_INITIALIZATION_WITH_PENDING_MODELIZATION/settings.json
--rw-rw-rw-   0        0        0      198 2022-08-23 08:03:11.350499 cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/import_0y1_INITIALIZATION_WITH_PENDING_MODELIZATION/status.json
--rw-rw-rw-   0        0        0     6659 2022-07-11 12:07:21.267583 cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/import_0y1_INITIALIZATION_WITH_PENDING_MODELIZATION/texts.json
--rw-rw-rw-   0        0        0        2 2022-07-11 12:07:21.312463 cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/import_0y2_INITIALIZATION_WITH_WORKING_MODELIZATION/clustering.json
--rw-rw-rw-   0        0        0        2 2022-07-11 12:07:21.271572 cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/import_0y2_INITIALIZATION_WITH_WORKING_MODELIZATION/constraints.json
--rw-rw-rw-   0        0        0      157 2022-07-29 10:05:16.190204 cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/import_0y2_INITIALIZATION_WITH_WORKING_MODELIZATION/metadata.json
--rw-rw-rw-   0        0        0     3045 2022-07-11 12:07:21.303486 cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/import_0y2_INITIALIZATION_WITH_WORKING_MODELIZATION/modelization.json
--rw-rw-rw-   0        0        0        2 2022-07-11 12:07:21.309471 cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/import_0y2_INITIALIZATION_WITH_WORKING_MODELIZATION/sampling.json
--rw-rw-rw-   0        0        0      696 2022-07-11 12:13:45.311609 cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/import_0y2_INITIALIZATION_WITH_WORKING_MODELIZATION/settings.json
--rw-rw-rw-   0        0        0      175 2022-08-23 08:03:11.350499 cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/import_0y2_INITIALIZATION_WITH_WORKING_MODELIZATION/status.json
--rw-rw-rw-   0        0        0     6659 2022-07-11 12:07:21.267583 cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/import_0y2_INITIALIZATION_WITH_WORKING_MODELIZATION/texts.json
--rw-rw-rw-   0        0        0      444 2022-07-29 09:18:22.863211 cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/import_1w0_IMPORT_AT_SAMPLING_STEP_WITHOUT_MODELIZATION/clustering.json
--rw-rw-rw-   0        0        0        2 2022-07-29 09:18:22.855235 cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/import_1w0_IMPORT_AT_SAMPLING_STEP_WITHOUT_MODELIZATION/constraints.json
--rw-rw-rw-   0        0        0      161 2022-07-29 10:14:43.461129 cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/import_1w0_IMPORT_AT_SAMPLING_STEP_WITHOUT_MODELIZATION/metadata.json
--rw-rw-rw-   0        0        0     3045 2022-07-29 09:18:22.868198 cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/import_1w0_IMPORT_AT_SAMPLING_STEP_WITHOUT_MODELIZATION/modelization.json
--rw-rw-rw-   0        0        0        2 2022-07-29 09:18:22.861216 cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/import_1w0_IMPORT_AT_SAMPLING_STEP_WITHOUT_MODELIZATION/sampling.json
--rw-rw-rw-   0        0        0     1580 2022-07-29 09:18:22.858225 cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/import_1w0_IMPORT_AT_SAMPLING_STEP_WITHOUT_MODELIZATION/settings.json
--rw-rw-rw-   0        0        0      108 2022-07-29 10:14:52.344716 cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/import_1w0_IMPORT_AT_SAMPLING_STEP_WITHOUT_MODELIZATION/status.json
--rw-rw-rw-   0        0        0     6513 2022-07-11 12:10:23.869094 cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/import_1w0_IMPORT_AT_SAMPLING_STEP_WITHOUT_MODELIZATION/texts.json
--rw-rw-rw-   0        0        0      444 2022-07-29 09:18:22.863211 cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/import_1w1_IMPORT_AT_SAMPLING_STEP_WITH_PENDING_MODELIZATION/clustering.json
--rw-rw-rw-   0        0        0        2 2022-07-29 09:18:22.855235 cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/import_1w1_IMPORT_AT_SAMPLING_STEP_WITH_PENDING_MODELIZATION/constraints.json
--rw-rw-rw-   0        0        0      166 2022-07-29 10:28:15.424848 cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/import_1w1_IMPORT_AT_SAMPLING_STEP_WITH_PENDING_MODELIZATION/metadata.json
--rw-rw-rw-   0        0        0     3045 2022-07-29 09:18:22.868198 cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/import_1w1_IMPORT_AT_SAMPLING_STEP_WITH_PENDING_MODELIZATION/modelization.json
--rw-rw-rw-   0        0        0        2 2022-07-29 09:18:22.861216 cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/import_1w1_IMPORT_AT_SAMPLING_STEP_WITH_PENDING_MODELIZATION/sampling.json
--rw-rw-rw-   0        0        0     1580 2022-07-29 09:18:22.858225 cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/import_1w1_IMPORT_AT_SAMPLING_STEP_WITH_PENDING_MODELIZATION/settings.json
--rw-rw-rw-   0        0        0      207 2022-08-23 08:03:11.350499 cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/import_1w1_IMPORT_AT_SAMPLING_STEP_WITH_PENDING_MODELIZATION/status.json
--rw-rw-rw-   0        0        0     6513 2022-07-11 12:10:23.869094 cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/import_1w1_IMPORT_AT_SAMPLING_STEP_WITH_PENDING_MODELIZATION/texts.json
--rw-rw-rw-   0        0        0      444 2022-07-29 09:18:22.863211 cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/import_1w2_IMPORT_AT_SAMPLING_STEP_WORKING_MODELIZATION/clustering.json
--rw-rw-rw-   0        0        0        2 2022-07-29 09:18:22.855235 cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/import_1w2_IMPORT_AT_SAMPLING_STEP_WORKING_MODELIZATION/constraints.json
--rw-rw-rw-   0        0        0      161 2022-07-29 10:26:02.398488 cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/import_1w2_IMPORT_AT_SAMPLING_STEP_WORKING_MODELIZATION/metadata.json
--rw-rw-rw-   0        0        0     3045 2022-07-29 09:18:22.868198 cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/import_1w2_IMPORT_AT_SAMPLING_STEP_WORKING_MODELIZATION/modelization.json
--rw-rw-rw-   0        0        0        2 2022-07-29 09:18:22.861216 cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/import_1w2_IMPORT_AT_SAMPLING_STEP_WORKING_MODELIZATION/sampling.json
--rw-rw-rw-   0        0        0     1580 2022-07-29 09:18:22.858225 cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/import_1w2_IMPORT_AT_SAMPLING_STEP_WORKING_MODELIZATION/settings.json
--rw-rw-rw-   0        0        0      184 2022-08-23 08:03:11.350499 cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/import_1w2_IMPORT_AT_SAMPLING_STEP_WORKING_MODELIZATION/status.json
--rw-rw-rw-   0        0        0     6513 2022-07-11 12:10:23.869094 cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/import_1w2_IMPORT_AT_SAMPLING_STEP_WORKING_MODELIZATION/texts.json
--rw-rw-rw-   0        0        0      444 2022-07-29 09:19:07.962559 cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/import_1x0_IMPORT_AT_ANNOTATION_STEP_WITHOUT_MODELIZATION/clustering.json
--rw-rw-rw-   0        0        0    11444 2022-07-11 13:32:13.084020 cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/import_1x0_IMPORT_AT_ANNOTATION_STEP_WITHOUT_MODELIZATION/constraints.json
--rw-rw-rw-   0        0        0      163 2022-07-29 10:16:34.037911 cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/import_1x0_IMPORT_AT_ANNOTATION_STEP_WITHOUT_MODELIZATION/metadata.json
--rw-rw-rw-   0        0        0     7676 2022-08-16 09:24:59.463501 cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/import_1x0_IMPORT_AT_ANNOTATION_STEP_WITHOUT_MODELIZATION/modelization.json
--rw-rw-rw-   0        0        0      498 2022-07-29 09:19:07.959568 cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/import_1x0_IMPORT_AT_ANNOTATION_STEP_WITHOUT_MODELIZATION/sampling.json
--rw-rw-rw-   0        0        0     1580 2022-07-29 09:19:07.956576 cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/import_1x0_IMPORT_AT_ANNOTATION_STEP_WITHOUT_MODELIZATION/settings.json
--rw-rw-rw-   0        0        0      110 2022-07-29 09:19:07.946602 cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/import_1x0_IMPORT_AT_ANNOTATION_STEP_WITHOUT_MODELIZATION/status.json
--rw-rw-rw-   0        0        0     6513 2022-07-11 12:10:23.869094 cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/import_1x0_IMPORT_AT_ANNOTATION_STEP_WITHOUT_MODELIZATION/texts.json
--rw-rw-rw-   0        0        0      444 2022-07-29 09:19:07.962559 cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/import_1x1_IMPORT_AT_ANNOTATION_STEP_WITH_PENDING_MODELIZATION/clustering.json
--rw-rw-rw-   0        0        0    11446 2022-08-16 08:43:22.934424 cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/import_1x1_IMPORT_AT_ANNOTATION_STEP_WITH_PENDING_MODELIZATION/constraints.json
--rw-rw-rw-   0        0        0      168 2022-07-29 10:28:42.145270 cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/import_1x1_IMPORT_AT_ANNOTATION_STEP_WITH_PENDING_MODELIZATION/metadata.json
--rw-rw-rw-   0        0        0     7676 2022-08-16 09:24:50.960133 cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/import_1x1_IMPORT_AT_ANNOTATION_STEP_WITH_PENDING_MODELIZATION/modelization.json
--rw-rw-rw-   0        0        0      498 2022-07-29 09:19:07.959568 cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/import_1x1_IMPORT_AT_ANNOTATION_STEP_WITH_PENDING_MODELIZATION/sampling.json
--rw-rw-rw-   0        0        0     1580 2022-07-29 09:19:07.956576 cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/import_1x1_IMPORT_AT_ANNOTATION_STEP_WITH_PENDING_MODELIZATION/settings.json
--rw-rw-rw-   0        0        0      209 2022-08-23 08:03:11.345513 cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/import_1x1_IMPORT_AT_ANNOTATION_STEP_WITH_PENDING_MODELIZATION/status.json
--rw-rw-rw-   0        0        0     6513 2022-07-11 12:10:23.869094 cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/import_1x1_IMPORT_AT_ANNOTATION_STEP_WITH_PENDING_MODELIZATION/texts.json
--rw-rw-rw-   0        0        0      444 2022-07-29 09:19:07.962559 cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/import_1x2_IMPORT_AT_ANNOTATION_STEP_WORKING_MODELIZATION/clustering.json
--rw-rw-rw-   0        0        0    11444 2022-07-11 13:32:13.084020 cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/import_1x2_IMPORT_AT_ANNOTATION_STEP_WORKING_MODELIZATION/constraints.json
--rw-rw-rw-   0        0        0      163 2022-07-29 10:26:35.966938 cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/import_1x2_IMPORT_AT_ANNOTATION_STEP_WORKING_MODELIZATION/metadata.json
--rw-rw-rw-   0        0        0     7676 2022-08-16 09:25:56.717172 cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/import_1x2_IMPORT_AT_ANNOTATION_STEP_WORKING_MODELIZATION/modelization.json
--rw-rw-rw-   0        0        0      498 2022-07-29 09:19:07.959568 cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/import_1x2_IMPORT_AT_ANNOTATION_STEP_WORKING_MODELIZATION/sampling.json
--rw-rw-rw-   0        0        0     1580 2022-07-29 09:19:07.956576 cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/import_1x2_IMPORT_AT_ANNOTATION_STEP_WORKING_MODELIZATION/settings.json
--rw-rw-rw-   0        0        0      186 2022-08-23 08:03:11.344515 cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/import_1x2_IMPORT_AT_ANNOTATION_STEP_WORKING_MODELIZATION/status.json
--rw-rw-rw-   0        0        0     6513 2022-07-11 12:10:23.869094 cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/import_1x2_IMPORT_AT_ANNOTATION_STEP_WORKING_MODELIZATION/texts.json
--rw-rw-rw-   0        0        0      444 2022-07-29 09:19:30.708376 cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/import_1y0_IMPORT_AT_CLUSTERING_STEP_WITHOUT_MODELIZATION/clustering.json
--rw-rw-rw-   0        0        0    11444 2022-07-29 09:19:30.702390 cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/import_1y0_IMPORT_AT_CLUSTERING_STEP_WITHOUT_MODELIZATION/constraints.json
--rw-rw-rw-   0        0        0      163 2022-07-29 10:16:45.014900 cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/import_1y0_IMPORT_AT_CLUSTERING_STEP_WITHOUT_MODELIZATION/metadata.json
--rw-rw-rw-   0        0        0     7676 2022-08-16 09:26:03.311603 cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/import_1y0_IMPORT_AT_CLUSTERING_STEP_WITHOUT_MODELIZATION/modelization.json
--rw-rw-rw-   0        0        0      498 2022-07-29 09:19:30.706380 cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/import_1y0_IMPORT_AT_CLUSTERING_STEP_WITHOUT_MODELIZATION/sampling.json
--rw-rw-rw-   0        0        0     1580 2022-07-29 09:19:30.704382 cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/import_1y0_IMPORT_AT_CLUSTERING_STEP_WITHOUT_MODELIZATION/settings.json
--rw-rw-rw-   0        0        0      110 2022-07-29 09:19:30.662979 cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/import_1y0_IMPORT_AT_CLUSTERING_STEP_WITHOUT_MODELIZATION/status.json
--rw-rw-rw-   0        0        0     6513 2022-07-11 12:10:23.869094 cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/import_1y0_IMPORT_AT_CLUSTERING_STEP_WITHOUT_MODELIZATION/texts.json
--rw-rw-rw-   0        0        0      444 2022-07-29 09:19:30.708376 cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/import_1y1_IMPORT_AT_CLUSTERING_STEP_WITH_PENDING_MODELIZATION/clustering.json
--rw-rw-rw-   0        0        0    11444 2022-07-29 09:19:30.702390 cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/import_1y1_IMPORT_AT_CLUSTERING_STEP_WITH_PENDING_MODELIZATION/constraints.json
--rw-rw-rw-   0        0        0      168 2022-07-29 10:28:57.082029 cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/import_1y1_IMPORT_AT_CLUSTERING_STEP_WITH_PENDING_MODELIZATION/metadata.json
--rw-rw-rw-   0        0        0     7676 2022-08-16 09:26:10.886957 cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/import_1y1_IMPORT_AT_CLUSTERING_STEP_WITH_PENDING_MODELIZATION/modelization.json
--rw-rw-rw-   0        0        0      498 2022-07-29 09:19:30.706380 cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/import_1y1_IMPORT_AT_CLUSTERING_STEP_WITH_PENDING_MODELIZATION/sampling.json
--rw-rw-rw-   0        0        0     1580 2022-07-29 09:19:30.704382 cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/import_1y1_IMPORT_AT_CLUSTERING_STEP_WITH_PENDING_MODELIZATION/settings.json
--rw-rw-rw-   0        0        0      209 2022-08-23 08:03:11.342520 cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/import_1y1_IMPORT_AT_CLUSTERING_STEP_WITH_PENDING_MODELIZATION/status.json
--rw-rw-rw-   0        0        0     6513 2022-07-11 12:10:23.869094 cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/import_1y1_IMPORT_AT_CLUSTERING_STEP_WITH_PENDING_MODELIZATION/texts.json
--rw-rw-rw-   0        0        0      444 2022-07-29 09:19:30.708376 cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/import_1y2_IMPORT_AT_CLUSTERING_STEP_WORKING_MODELIZATION/clustering.json
--rw-rw-rw-   0        0        0    11444 2022-07-29 09:19:30.702390 cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/import_1y2_IMPORT_AT_CLUSTERING_STEP_WORKING_MODELIZATION/constraints.json
--rw-rw-rw-   0        0        0      163 2022-07-29 10:26:51.304470 cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/import_1y2_IMPORT_AT_CLUSTERING_STEP_WORKING_MODELIZATION/metadata.json
--rw-rw-rw-   0        0        0     7676 2022-08-16 09:26:18.210742 cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/import_1y2_IMPORT_AT_CLUSTERING_STEP_WORKING_MODELIZATION/modelization.json
--rw-rw-rw-   0        0        0      498 2022-07-29 09:19:30.706380 cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/import_1y2_IMPORT_AT_CLUSTERING_STEP_WORKING_MODELIZATION/sampling.json
--rw-rw-rw-   0        0        0     1580 2022-07-29 09:19:30.704382 cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/import_1y2_IMPORT_AT_CLUSTERING_STEP_WORKING_MODELIZATION/settings.json
--rw-rw-rw-   0        0        0      186 2022-08-23 08:03:11.338532 cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/import_1y2_IMPORT_AT_CLUSTERING_STEP_WORKING_MODELIZATION/status.json
--rw-rw-rw-   0        0        0     6513 2022-07-11 12:10:23.869094 cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/import_1y2_IMPORT_AT_CLUSTERING_STEP_WORKING_MODELIZATION/texts.json
--rw-rw-rw-   0        0        0      867 2022-07-29 09:19:45.960931 cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/import_1z0_IMPORT_AT_ITERATION_END_WITHOUT_MODELIZATION/clustering.json
--rw-rw-rw-   0        0        0    11444 2022-07-29 09:19:45.951958 cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/import_1z0_IMPORT_AT_ITERATION_END_WITHOUT_MODELIZATION/constraints.json
--rw-rw-rw-   0        0        0      161 2022-07-29 10:17:15.766568 cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/import_1z0_IMPORT_AT_ITERATION_END_WITHOUT_MODELIZATION/metadata.json
--rw-rw-rw-   0        0        0     7676 2022-08-16 09:26:25.021358 cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/import_1z0_IMPORT_AT_ITERATION_END_WITHOUT_MODELIZATION/modelization.json
--rw-rw-rw-   0        0        0      498 2022-07-29 09:19:45.957939 cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/import_1z0_IMPORT_AT_ITERATION_END_WITHOUT_MODELIZATION/sampling.json
--rw-rw-rw-   0        0        0     1580 2022-07-29 09:19:45.954954 cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/import_1z0_IMPORT_AT_ITERATION_END_WITHOUT_MODELIZATION/settings.json
--rw-rw-rw-   0        0        0      108 2022-07-29 09:19:45.942978 cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/import_1z0_IMPORT_AT_ITERATION_END_WITHOUT_MODELIZATION/status.json
--rw-rw-rw-   0        0        0     6513 2022-07-11 12:10:23.869094 cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/import_1z0_IMPORT_AT_ITERATION_END_WITHOUT_MODELIZATION/texts.json
--rw-rw-rw-   0        0        0      867 2022-08-16 08:30:23.075267 cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/import_1z1_IMPORT_AT_ITERATION_END_WITH_PENDING_MODELIZATION/clustering.json
--rw-rw-rw-   0        0        0    11444 2022-07-29 09:19:45.951958 cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/import_1z1_IMPORT_AT_ITERATION_END_WITH_PENDING_MODELIZATION/constraints.json
--rw-rw-rw-   0        0        0      166 2022-07-29 10:29:09.786464 cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/import_1z1_IMPORT_AT_ITERATION_END_WITH_PENDING_MODELIZATION/metadata.json
--rw-rw-rw-   0        0        0     7676 2022-08-16 09:26:32.211112 cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/import_1z1_IMPORT_AT_ITERATION_END_WITH_PENDING_MODELIZATION/modelization.json
--rw-rw-rw-   0        0        0      498 2022-07-29 09:19:45.957939 cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/import_1z1_IMPORT_AT_ITERATION_END_WITH_PENDING_MODELIZATION/sampling.json
--rw-rw-rw-   0        0        0     1580 2022-07-29 09:19:45.954954 cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/import_1z1_IMPORT_AT_ITERATION_END_WITH_PENDING_MODELIZATION/settings.json
--rw-rw-rw-   0        0        0      207 2022-08-23 08:03:11.338532 cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/import_1z1_IMPORT_AT_ITERATION_END_WITH_PENDING_MODELIZATION/status.json
--rw-rw-rw-   0        0        0     6513 2022-07-11 12:10:23.869094 cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/import_1z1_IMPORT_AT_ITERATION_END_WITH_PENDING_MODELIZATION/texts.json
--rw-rw-rw-   0        0        0      867 2022-07-29 09:19:45.960931 cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/import_1z2_IMPORT_AT_ITERATION_END_WORKING_MODELIZATION/clustering.json
--rw-rw-rw-   0        0        0    11444 2022-07-29 09:19:45.951958 cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/import_1z2_IMPORT_AT_ITERATION_END_WORKING_MODELIZATION/constraints.json
--rw-rw-rw-   0        0        0      161 2022-07-29 10:27:07.008169 cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/import_1z2_IMPORT_AT_ITERATION_END_WORKING_MODELIZATION/metadata.json
--rw-rw-rw-   0        0        0     7676 2022-08-16 09:26:39.280399 cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/import_1z2_IMPORT_AT_ITERATION_END_WORKING_MODELIZATION/modelization.json
--rw-rw-rw-   0        0        0      498 2022-07-29 09:19:45.957939 cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/import_1z2_IMPORT_AT_ITERATION_END_WORKING_MODELIZATION/sampling.json
--rw-rw-rw-   0        0        0     1580 2022-07-29 09:19:45.954954 cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/import_1z2_IMPORT_AT_ITERATION_END_WORKING_MODELIZATION/settings.json
--rw-rw-rw-   0        0        0      184 2022-08-23 08:03:11.338532 cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/import_1z2_IMPORT_AT_ITERATION_END_WORKING_MODELIZATION/status.json
--rw-rw-rw-   0        0        0     6513 2022-07-11 12:10:23.869094 cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/import_1z2_IMPORT_AT_ITERATION_END_WORKING_MODELIZATION/texts.json
--rw-rw-rw-   0        0        0        2 2022-07-11 12:07:21.312463 cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/import_error_0y1_INITIALIZATION_WITH_PENDING_MODELIZATION/clustering.json
--rw-rw-rw-   0        0        0     1810 2022-07-29 10:12:35.231746 cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/import_error_0y1_INITIALIZATION_WITH_PENDING_MODELIZATION/constraints.json
--rw-rw-rw-   0        0        0      163 2022-07-29 10:07:25.679543 cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/import_error_0y1_INITIALIZATION_WITH_PENDING_MODELIZATION/metadata.json
--rw-rw-rw-   0        0        0     3045 2022-07-11 12:07:21.303486 cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/import_error_0y1_INITIALIZATION_WITH_PENDING_MODELIZATION/modelization.json
--rw-rw-rw-   0        0        0        2 2022-07-11 12:07:21.309471 cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/import_error_0y1_INITIALIZATION_WITH_PENDING_MODELIZATION/sampling.json
--rw-rw-rw-   0        0        0      696 2022-07-11 12:13:45.311609 cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/import_error_0y1_INITIALIZATION_WITH_PENDING_MODELIZATION/settings.json
--rw-rw-rw-   0        0        0      198 2022-08-23 08:03:11.333544 cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/import_error_0y1_INITIALIZATION_WITH_PENDING_MODELIZATION/status.json
--rw-rw-rw-   0        0        0     6659 2022-08-16 08:35:06.321495 cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/import_error_0y1_INITIALIZATION_WITH_PENDING_MODELIZATION/texts.json
--rw-rw-rw-   0        0        0        2 2022-07-11 12:07:21.312463 cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/import_error_0y3_INITIALIZATION_WITH_ERRORS/clustering.json
--rw-rw-rw-   0        0        0     1809 2022-07-29 11:06:31.807149 cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/import_error_0y3_INITIALIZATION_WITH_ERRORS/constraints.json
--rw-rw-rw-   0        0        0     1952 2022-08-23 13:18:42.129355 cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/import_error_0y3_INITIALIZATION_WITH_ERRORS/constraints_manager.pkl
--rw-rw-rw-   0        0        0      149 2022-07-29 11:03:08.541867 cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/import_error_0y3_INITIALIZATION_WITH_ERRORS/metadata.json
--rw-rw-rw-   0        0        0     3295 2022-07-29 11:06:32.237676 cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/import_error_0y3_INITIALIZATION_WITH_ERRORS/modelization.json
--rw-rw-rw-   0        0        0        2 2022-07-11 12:07:21.309471 cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/import_error_0y3_INITIALIZATION_WITH_ERRORS/sampling.json
--rw-rw-rw-   0        0        0      696 2022-07-11 12:13:45.311609 cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/import_error_0y3_INITIALIZATION_WITH_ERRORS/settings.json
--rw-rw-rw-   0        0        0       90 2022-07-29 11:06:32.250642 cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/import_error_0y3_INITIALIZATION_WITH_ERRORS/status.json
--rw-rw-rw-   0        0        0     6659 2022-08-16 08:35:15.548914 cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/import_error_0y3_INITIALIZATION_WITH_ERRORS/texts.json
--rw-rw-rw-   0        0        0     5825 2022-07-29 11:06:29.081110 cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/import_error_0y3_INITIALIZATION_WITH_ERRORS/vectors.pkl
--rw-rw-rw-   0        0        0     2106 2022-07-29 11:06:30.058680 cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/import_error_0y3_INITIALIZATION_WITH_ERRORS/vectors_2D.json
--rw-rw-rw-   0        0        0     2904 2022-07-29 11:06:31.334405 cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/import_error_0y3_INITIALIZATION_WITH_ERRORS/vectors_3D.json
--rw-rw-rw-   0        0        0      444 2022-08-16 08:29:07.499761 cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/import_error_1w1_IMPORT_AT_SAMPLING_STEP_WITH_PENDING_MODELIZATION/clustering.json
--rw-rw-rw-   0        0        0     1810 2022-07-29 10:12:35.231746 cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/import_error_1w1_IMPORT_AT_SAMPLING_STEP_WITH_PENDING_MODELIZATION/constraints.json
--rw-rw-rw-   0        0        0      163 2022-07-29 10:07:25.679543 cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/import_error_1w1_IMPORT_AT_SAMPLING_STEP_WITH_PENDING_MODELIZATION/metadata.json
--rw-rw-rw-   0        0        0     3045 2022-07-11 12:07:21.303486 cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/import_error_1w1_IMPORT_AT_SAMPLING_STEP_WITH_PENDING_MODELIZATION/modelization.json
--rw-rw-rw-   0        0        0        2 2022-07-11 12:07:21.309471 cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/import_error_1w1_IMPORT_AT_SAMPLING_STEP_WITH_PENDING_MODELIZATION/sampling.json
--rw-rw-rw-   0        0        0     1580 2022-08-16 08:27:13.966013 cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/import_error_1w1_IMPORT_AT_SAMPLING_STEP_WITH_PENDING_MODELIZATION/settings.json
--rw-rw-rw-   0        0        0      207 2022-08-23 08:03:11.333544 cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/import_error_1w1_IMPORT_AT_SAMPLING_STEP_WITH_PENDING_MODELIZATION/status.json
--rw-rw-rw-   0        0        0     6513 2022-07-11 12:10:23.869094 cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/import_error_1w1_IMPORT_AT_SAMPLING_STEP_WITH_PENDING_MODELIZATION/texts.json
--rw-rw-rw-   0        0        0      444 2022-08-16 08:29:14.945429 cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/import_error_1w3_IMPORT_AT_SAMPLING_STEP_WITH_ERRORS/clustering.json
--rw-rw-rw-   0        0        0     1809 2022-07-29 11:07:16.025511 cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/import_error_1w3_IMPORT_AT_SAMPLING_STEP_WITH_ERRORS/constraints.json
--rw-rw-rw-   0        0        0     1952 2022-08-23 13:18:42.136334 cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/import_error_1w3_IMPORT_AT_SAMPLING_STEP_WITH_ERRORS/constraints_manager.pkl
--rw-rw-rw-   0        0        0      158 2022-07-29 11:03:25.478398 cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/import_error_1w3_IMPORT_AT_SAMPLING_STEP_WITH_ERRORS/metadata.json
--rw-rw-rw-   0        0        0     3295 2022-07-29 11:07:16.516888 cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/import_error_1w3_IMPORT_AT_SAMPLING_STEP_WITH_ERRORS/modelization.json
--rw-rw-rw-   0        0        0        2 2022-07-11 12:07:21.309471 cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/import_error_1w3_IMPORT_AT_SAMPLING_STEP_WITH_ERRORS/sampling.json
--rw-rw-rw-   0        0        0     1580 2022-08-16 08:27:27.996356 cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/import_error_1w3_IMPORT_AT_SAMPLING_STEP_WITH_ERRORS/settings.json
--rw-rw-rw-   0        0        0       99 2022-07-29 14:59:58.636777 cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/import_error_1w3_IMPORT_AT_SAMPLING_STEP_WITH_ERRORS/status.json
--rw-rw-rw-   0        0        0     6513 2022-07-29 11:07:05.483900 cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/import_error_1w3_IMPORT_AT_SAMPLING_STEP_WITH_ERRORS/texts.json
--rw-rw-rw-   0        0        0     5825 2022-07-29 11:07:06.474279 cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/import_error_1w3_IMPORT_AT_SAMPLING_STEP_WITH_ERRORS/vectors.pkl
--rw-rw-rw-   0        0        0     2106 2022-07-29 11:07:12.409116 cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/import_error_1w3_IMPORT_AT_SAMPLING_STEP_WITH_ERRORS/vectors_2D.json
--rw-rw-rw-   0        0        0     2904 2022-07-29 11:07:15.505121 cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/import_error_1w3_IMPORT_AT_SAMPLING_STEP_WITH_ERRORS/vectors_3D.json
--rw-rw-rw-   0        0        0      444 2022-08-16 08:29:35.853846 cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/import_error_1x1_IMPORT_AT_ANNOTATION_STEP_WITH_PENDING_MODELIZATION/clustering.json
--rw-rw-rw-   0        0        0     1810 2022-07-29 10:12:35.231746 cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/import_error_1x1_IMPORT_AT_ANNOTATION_STEP_WITH_PENDING_MODELIZATION/constraints.json
--rw-rw-rw-   0        0        0      163 2022-07-29 10:07:25.679543 cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/import_error_1x1_IMPORT_AT_ANNOTATION_STEP_WITH_PENDING_MODELIZATION/metadata.json
--rw-rw-rw-   0        0        0     3045 2022-07-11 12:07:21.303486 cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/import_error_1x1_IMPORT_AT_ANNOTATION_STEP_WITH_PENDING_MODELIZATION/modelization.json
--rw-rw-rw-   0        0        0        2 2022-07-11 12:07:21.309471 cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/import_error_1x1_IMPORT_AT_ANNOTATION_STEP_WITH_PENDING_MODELIZATION/sampling.json
--rw-rw-rw-   0        0        0     1580 2022-08-16 08:27:38.472320 cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/import_error_1x1_IMPORT_AT_ANNOTATION_STEP_WITH_PENDING_MODELIZATION/settings.json
--rw-rw-rw-   0        0        0      209 2022-08-23 08:03:11.331549 cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/import_error_1x1_IMPORT_AT_ANNOTATION_STEP_WITH_PENDING_MODELIZATION/status.json
--rw-rw-rw-   0        0        0     6513 2022-07-11 12:10:23.869094 cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/import_error_1x1_IMPORT_AT_ANNOTATION_STEP_WITH_PENDING_MODELIZATION/texts.json
--rw-rw-rw-   0        0        0      444 2022-08-16 08:29:43.768715 cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/import_error_1x3_ANNOTATION_WITH_OUTDATED_MODELIZATION_WITH_CONFLICTS/clustering.json
--rw-rw-rw-   0        0        0     1809 2022-07-29 11:07:37.951319 cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/import_error_1x3_ANNOTATION_WITH_OUTDATED_MODELIZATION_WITH_CONFLICTS/constraints.json
--rw-rw-rw-   0        0        0     1952 2022-08-23 13:18:42.143315 cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/import_error_1x3_ANNOTATION_WITH_OUTDATED_MODELIZATION_WITH_CONFLICTS/constraints_manager.pkl
--rw-rw-rw-   0        0        0      175 2022-07-29 11:03:59.823007 cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/import_error_1x3_ANNOTATION_WITH_OUTDATED_MODELIZATION_WITH_CONFLICTS/metadata.json
--rw-rw-rw-   0        0        0     3295 2022-07-29 11:07:38.406161 cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/import_error_1x3_ANNOTATION_WITH_OUTDATED_MODELIZATION_WITH_CONFLICTS/modelization.json
--rw-rw-rw-   0        0        0        2 2022-07-11 12:07:21.309471 cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/import_error_1x3_ANNOTATION_WITH_OUTDATED_MODELIZATION_WITH_CONFLICTS/sampling.json
--rw-rw-rw-   0        0        0     1580 2022-08-16 08:27:46.098266 cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/import_error_1x3_ANNOTATION_WITH_OUTDATED_MODELIZATION_WITH_CONFLICTS/settings.json
--rw-rw-rw-   0        0        0      116 2022-07-29 15:00:54.721230 cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/import_error_1x3_ANNOTATION_WITH_OUTDATED_MODELIZATION_WITH_CONFLICTS/status.json
--rw-rw-rw-   0        0        0     6513 2022-07-29 11:07:35.037212 cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/import_error_1x3_ANNOTATION_WITH_OUTDATED_MODELIZATION_WITH_CONFLICTS/texts.json
--rw-rw-rw-   0        0        0     5825 2022-07-29 11:07:35.496991 cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/import_error_1x3_ANNOTATION_WITH_OUTDATED_MODELIZATION_WITH_CONFLICTS/vectors.pkl
--rw-rw-rw-   0        0        0     2106 2022-07-29 11:07:36.384630 cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/import_error_1x3_ANNOTATION_WITH_OUTDATED_MODELIZATION_WITH_CONFLICTS/vectors_2D.json
--rw-rw-rw-   0        0        0     2904 2022-07-29 11:07:37.453644 cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/import_error_1x3_ANNOTATION_WITH_OUTDATED_MODELIZATION_WITH_CONFLICTS/vectors_3D.json
--rw-rw-rw-   0        0        0      444 2022-08-16 08:29:48.698371 cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/import_error_1y1_IMPORT_AT_CLUSTERING_STEP_WITH_PENDING_MODELIZATION/clustering.json
--rw-rw-rw-   0        0        0     1810 2022-07-29 10:12:35.231746 cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/import_error_1y1_IMPORT_AT_CLUSTERING_STEP_WITH_PENDING_MODELIZATION/constraints.json
--rw-rw-rw-   0        0        0      163 2022-07-29 10:07:25.679543 cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/import_error_1y1_IMPORT_AT_CLUSTERING_STEP_WITH_PENDING_MODELIZATION/metadata.json
--rw-rw-rw-   0        0        0     3045 2022-07-11 12:07:21.303486 cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/import_error_1y1_IMPORT_AT_CLUSTERING_STEP_WITH_PENDING_MODELIZATION/modelization.json
--rw-rw-rw-   0        0        0        2 2022-07-11 12:07:21.309471 cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/import_error_1y1_IMPORT_AT_CLUSTERING_STEP_WITH_PENDING_MODELIZATION/sampling.json
--rw-rw-rw-   0        0        0     1580 2022-08-16 08:27:52.228290 cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/import_error_1y1_IMPORT_AT_CLUSTERING_STEP_WITH_PENDING_MODELIZATION/settings.json
--rw-rw-rw-   0        0        0      209 2022-08-23 08:03:11.325564 cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/import_error_1y1_IMPORT_AT_CLUSTERING_STEP_WITH_PENDING_MODELIZATION/status.json
--rw-rw-rw-   0        0        0     6513 2022-07-11 12:10:23.869094 cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/import_error_1y1_IMPORT_AT_CLUSTERING_STEP_WITH_PENDING_MODELIZATION/texts.json
--rw-rw-rw-   0        0        0        2 2022-07-11 12:07:21.312463 cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/import_error_1y3_IMPORT_AT_CLUSTERING_STEP_WITH_ERRORS/clustering.json
--rw-rw-rw-   0        0        0     1809 2022-07-29 11:08:01.407612 cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/import_error_1y3_IMPORT_AT_CLUSTERING_STEP_WITH_ERRORS/constraints.json
--rw-rw-rw-   0        0        0     1952 2022-08-23 13:18:42.150300 cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/import_error_1y3_IMPORT_AT_CLUSTERING_STEP_WITH_ERRORS/constraints_manager.pkl
--rw-rw-rw-   0        0        0      160 2022-07-29 11:04:53.647016 cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/import_error_1y3_IMPORT_AT_CLUSTERING_STEP_WITH_ERRORS/metadata.json
--rw-rw-rw-   0        0        0     3295 2022-07-29 11:08:01.848439 cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/import_error_1y3_IMPORT_AT_CLUSTERING_STEP_WITH_ERRORS/modelization.json
--rw-rw-rw-   0        0        0        2 2022-07-11 12:07:21.309471 cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/import_error_1y3_IMPORT_AT_CLUSTERING_STEP_WITH_ERRORS/sampling.json
--rw-rw-rw-   0        0        0     1580 2022-08-16 08:27:57.792616 cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/import_error_1y3_IMPORT_AT_CLUSTERING_STEP_WITH_ERRORS/settings.json
--rw-rw-rw-   0        0        0      101 2022-07-29 15:00:30.036260 cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/import_error_1y3_IMPORT_AT_CLUSTERING_STEP_WITH_ERRORS/status.json
--rw-rw-rw-   0        0        0     6513 2022-07-29 11:07:57.236796 cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/import_error_1y3_IMPORT_AT_CLUSTERING_STEP_WITH_ERRORS/texts.json
--rw-rw-rw-   0        0        0     5825 2022-07-29 11:07:57.866120 cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/import_error_1y3_IMPORT_AT_CLUSTERING_STEP_WITH_ERRORS/vectors.pkl
--rw-rw-rw-   0        0        0     2106 2022-07-29 11:07:58.905499 cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/import_error_1y3_IMPORT_AT_CLUSTERING_STEP_WITH_ERRORS/vectors_2D.json
--rw-rw-rw-   0        0        0     2904 2022-07-29 11:08:00.851094 cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/import_error_1y3_IMPORT_AT_CLUSTERING_STEP_WITH_ERRORS/vectors_3D.json
--rw-rw-rw-   0        0        0      867 2022-08-16 08:30:39.719787 cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/import_error_1z1_IMPORT_AT_ITERATION_END_WITH_PENDING_MODELIZATION/clustering.json
--rw-rw-rw-   0        0        0     1810 2022-07-29 10:12:35.231746 cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/import_error_1z1_IMPORT_AT_ITERATION_END_WITH_PENDING_MODELIZATION/constraints.json
--rw-rw-rw-   0        0        0      163 2022-07-29 10:07:25.679543 cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/import_error_1z1_IMPORT_AT_ITERATION_END_WITH_PENDING_MODELIZATION/metadata.json
--rw-rw-rw-   0        0        0     3045 2022-07-11 12:07:21.303486 cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/import_error_1z1_IMPORT_AT_ITERATION_END_WITH_PENDING_MODELIZATION/modelization.json
--rw-rw-rw-   0        0        0        2 2022-07-11 12:07:21.309471 cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/import_error_1z1_IMPORT_AT_ITERATION_END_WITH_PENDING_MODELIZATION/sampling.json
--rw-rw-rw-   0        0        0     1580 2022-08-16 08:28:02.649641 cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/import_error_1z1_IMPORT_AT_ITERATION_END_WITH_PENDING_MODELIZATION/settings.json
--rw-rw-rw-   0        0        0      207 2022-08-23 08:03:11.325564 cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/import_error_1z1_IMPORT_AT_ITERATION_END_WITH_PENDING_MODELIZATION/status.json
--rw-rw-rw-   0        0        0     6513 2022-07-11 12:10:23.869094 cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/import_error_1z1_IMPORT_AT_ITERATION_END_WITH_PENDING_MODELIZATION/texts.json
--rw-rw-rw-   0        0        0      867 2022-08-16 08:30:33.193314 cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/import_error_1z3_IMPORT_AT_ITERATION_END_WITH_ERRORS/clustering.json
--rw-rw-rw-   0        0        0     1809 2022-07-29 11:08:29.596577 cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/import_error_1z3_IMPORT_AT_ITERATION_END_WITH_ERRORS/constraints.json
--rw-rw-rw-   0        0        0     1952 2022-08-23 13:18:42.156284 cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/import_error_1z3_IMPORT_AT_ITERATION_END_WITH_ERRORS/constraints_manager.pkl
--rw-rw-rw-   0        0        0      158 2022-07-29 11:05:26.855897 cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/import_error_1z3_IMPORT_AT_ITERATION_END_WITH_ERRORS/metadata.json
--rw-rw-rw-   0        0        0     3295 2022-07-29 11:08:30.039362 cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/import_error_1z3_IMPORT_AT_ITERATION_END_WITH_ERRORS/modelization.json
--rw-rw-rw-   0        0        0        2 2022-07-11 12:07:21.309471 cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/import_error_1z3_IMPORT_AT_ITERATION_END_WITH_ERRORS/sampling.json
--rw-rw-rw-   0        0        0     1580 2022-08-16 08:28:08.092799 cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/import_error_1z3_IMPORT_AT_ITERATION_END_WITH_ERRORS/settings.json
--rw-rw-rw-   0        0        0       99 2022-07-29 15:01:48.266216 cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/import_error_1z3_IMPORT_AT_ITERATION_END_WITH_ERRORS/status.json
--rw-rw-rw-   0        0        0     6513 2022-07-29 11:08:24.466061 cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/import_error_1z3_IMPORT_AT_ITERATION_END_WITH_ERRORS/texts.json
--rw-rw-rw-   0        0        0     5825 2022-07-29 11:08:24.936923 cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/import_error_1z3_IMPORT_AT_ITERATION_END_WITH_ERRORS/vectors.pkl
--rw-rw-rw-   0        0        0     2106 2022-07-29 11:08:26.680342 cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/import_error_1z3_IMPORT_AT_ITERATION_END_WITH_ERRORS/vectors_2D.json
--rw-rw-rw-   0        0        0     2904 2022-07-29 11:08:29.027093 cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/import_error_1z3_IMPORT_AT_ITERATION_END_WITH_ERRORS/vectors_3D.json
--rw-rw-rw-   0        0        0     6116 2022-08-16 13:42:46.875108 cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies_utils.py
--rw-rw-rw-   0        0        0      858 2022-08-22 15:59:06.845649 cognitivefactory-interactive-clustering-gui-0.4.0/tests/test_app.py
--rw-rw-rw-   0        0        0      971 2022-08-23 07:48:17.781994 cognitivefactory-interactive-clustering-gui-0.4.0/tests/test_backgroundtasks.py
--rw-rw-rw-   0        0        0     1093 2022-08-26 15:44:17.408153 cognitivefactory-interactive-clustering-gui-0.4.0/tests/test_cli.py
--rw-rw-rw-   0        0        0     3230 2022-08-23 11:37:04.834986 cognitivefactory-interactive-clustering-gui-0.4.0/tests/test_delete_api_projects.py
--rw-rw-rw-   0        0        0     1062 2022-07-22 13:34:01.176251 cognitivefactory-interactive-clustering-gui-0.4.0/tests/test_get_alive.py
--rw-rw-rw-   0        0        0     2606 2022-07-25 14:31:40.122180 cognitivefactory-interactive-clustering-gui-0.4.0/tests/test_get_api_projects.py
--rw-rw-rw-   0        0        0    10271 2022-07-26 09:10:34.242910 cognitivefactory-interactive-clustering-gui-0.4.0/tests/test_get_api_projects_clustering.py
--rw-rw-rw-   0        0        0   203926 2022-08-18 15:15:28.910254 cognitivefactory-interactive-clustering-gui-0.4.0/tests/test_get_api_projects_constraints.py
--rw-rw-rw-   0        0        0     4054 2022-07-25 14:53:28.619212 cognitivefactory-interactive-clustering-gui-0.4.0/tests/test_get_api_projects_download.py
--rw-rw-rw-   0        0        0     3047 2022-07-28 06:34:57.853635 cognitivefactory-interactive-clustering-gui-0.4.0/tests/test_get_api_projects_metadata.py
--rw-rw-rw-   0        0        0    10686 2022-07-25 14:15:53.467482 cognitivefactory-interactive-clustering-gui-0.4.0/tests/test_get_api_projects_modelization.py
--rw-rw-rw-   0        0        0    18434 2022-08-18 13:29:11.062683 cognitivefactory-interactive-clustering-gui-0.4.0/tests/test_get_api_projects_sampling.py
--rw-rw-rw-   0        0        0    13930 2022-08-18 13:29:08.531336 cognitivefactory-interactive-clustering-gui-0.4.0/tests/test_get_api_projects_settings.py
--rw-rw-rw-   0        0        0     5411 2022-08-23 08:03:48.974293 cognitivefactory-interactive-clustering-gui-0.4.0/tests/test_get_api_projects_status.py
--rw-rw-rw-   0        0        0    53392 2022-07-25 14:10:08.984923 cognitivefactory-interactive-clustering-gui-0.4.0/tests/test_get_api_projects_texts.py
--rw-rw-rw-   0        0        0     9477 2022-07-27 07:14:13.049815 cognitivefactory-interactive-clustering-gui-0.4.0/tests/test_get_api_projects_vectors.py
--rw-rw-rw-   0        0        0     1081 2022-07-22 13:33:57.668268 cognitivefactory-interactive-clustering-gui-0.4.0/tests/test_get_gui_help.py
--rw-rw-rw-   0        0        0     7987 2022-07-26 08:01:48.258129 cognitivefactory-interactive-clustering-gui-0.4.0/tests/test_get_gui_projects_constraints.py
--rw-rw-rw-   0        0        0    10312 2022-07-27 08:11:56.167878 cognitivefactory-interactive-clustering-gui-0.4.0/tests/test_get_gui_projects_constraints_annotation.py
--rw-rw-rw-   0        0        0     9317 2022-07-25 14:31:40.122180 cognitivefactory-interactive-clustering-gui-0.4.0/tests/test_get_gui_projects_home.py
--rw-rw-rw-   0        0        0     6789 2022-07-29 14:50:33.631265 cognitivefactory-interactive-clustering-gui-0.4.0/tests/test_get_gui_projects_listing.py
--rw-rw-rw-   0        0        0    13315 2022-07-27 07:23:07.286328 cognitivefactory-interactive-clustering-gui-0.4.0/tests/test_get_gui_projects_settings.py
--rw-rw-rw-   0        0        0     7706 2022-07-25 14:53:16.989570 cognitivefactory-interactive-clustering-gui-0.4.0/tests/test_get_gui_projects_texts.py
--rw-rw-rw-   0        0        0      935 2022-07-25 14:57:11.394414 cognitivefactory-interactive-clustering-gui-0.4.0/tests/test_get_ready.py
--rw-rw-rw-   0        0        0     1048 2022-08-31 15:09:00.725396 cognitivefactory-interactive-clustering-gui-0.4.0/tests/test_get_welcome.py
--rw-rw-rw-   0        0        0    11755 2022-08-22 15:59:06.841665 cognitivefactory-interactive-clustering-gui-0.4.0/tests/test_post_api_projects.py
--rw-rw-rw-   0        0        0     9996 2022-08-23 14:15:24.749320 cognitivefactory-interactive-clustering-gui-0.4.0/tests/test_post_api_projects_clustering.py
--rw-rw-rw-   0        0        0    11389 2022-07-26 13:50:01.419643 cognitivefactory-interactive-clustering-gui-0.4.0/tests/test_post_api_projects_constraints_approve.py
--rw-rw-rw-   0        0        0    10398 2022-07-25 14:34:47.900760 cognitivefactory-interactive-clustering-gui-0.4.0/tests/test_post_api_projects_iterations.py
--rw-rw-rw-   0        0        0    24960 2022-08-24 09:11:46.541829 cognitivefactory-interactive-clustering-gui-0.4.0/tests/test_post_api_projects_modelization.py
--rw-rw-rw-   0        0        0    10030 2022-08-24 09:12:45.857916 cognitivefactory-interactive-clustering-gui-0.4.0/tests/test_post_api_projects_sampling.py
--rw-rw-rw-   0        0        0    24426 2022-07-25 14:52:59.709528 cognitivefactory-interactive-clustering-gui-0.4.0/tests/test_put_api_projects.py
--rw-rw-rw-   0        0        0    25890 2022-07-26 13:50:01.413659 cognitivefactory-interactive-clustering-gui-0.4.0/tests/test_put_api_projects_constraints_annotate.py
--rw-rw-rw-   0        0        0     9038 2022-07-26 13:50:01.415654 cognitivefactory-interactive-clustering-gui-0.4.0/tests/test_put_api_projects_constraints_comment.py
--rw-rw-rw-   0        0        0    11185 2022-07-26 13:50:01.408678 cognitivefactory-interactive-clustering-gui-0.4.0/tests/test_put_api_projects_constraints_review.py
--rw-rw-rw-   0        0        0    76179 2022-07-27 11:39:00.153602 cognitivefactory-interactive-clustering-gui-0.4.0/tests/test_put_api_projects_settings.py
--rw-rw-rw-   0        0        0    20464 2022-07-26 13:53:12.255355 cognitivefactory-interactive-clustering-gui-0.4.0/tests/test_put_api_projects_texts_delete.py
--rw-rw-rw-   0        0        0    18904 2022-07-26 13:53:26.121350 cognitivefactory-interactive-clustering-gui-0.4.0/tests/test_put_api_projects_texts_rename.py
--rw-rw-rw-   0        0        0    20442 2022-07-26 13:52:57.711966 cognitivefactory-interactive-clustering-gui-0.4.0/tests/test_put_api_projects_texts_undelete.py
--rw-rw-rw-   0        0        0     7155 2022-08-23 14:21:58.860410 cognitivefactory-interactive-clustering-gui-0.4.0/tests/test_run_constrained_clustering_task.py
--rw-rw-rw-   0        0        0    23297 2022-08-23 14:21:58.891658 cognitivefactory-interactive-clustering-gui-0.4.0/tests/test_run_constraints_sampling_task.py
--rw-rw-rw-   0        0        0   311634 2022-08-23 14:21:59.125982 cognitivefactory-interactive-clustering-gui-0.4.0/tests/test_run_modelization_update_task.py
--rw-rw-rw-   0        0        0     2906 2022-08-22 17:41:44.848998 cognitivefactory-interactive-clustering-gui-0.4.0/tests/test_utils_jinja_filters.py
--rw-rw-rw-   0        0        0     1193 2022-08-22 15:59:06.825664 cognitivefactory-interactive-clustering-gui-0.4.0/tests/test_utils_models_settings.py
--rw-rw-rw-   0        0        0     1229 2022-08-22 15:59:06.823669 cognitivefactory-interactive-clustering-gui-0.4.0/tests/test_utils_models_states.py
--rw-rw-rw-   0        0        0     7615 2022-09-01 09:47:04.102213 cognitivefactory-interactive-clustering-gui-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0    22748 2022-08-18 15:35:45.547399 cognitivefactory-interactive-clustering-gui-0.4.1/LICENSE.md
+-rw-r--r--   0        0        0     4187 2023-02-16 17:55:52.909695 cognitivefactory-interactive-clustering-gui-0.4.1/pyproject.toml
+-rw-r--r--   0        0        0     5140 2023-02-16 15:28:31.290968 cognitivefactory-interactive-clustering-gui-0.4.1/README.md
+-rw-r--r--   0        0        0      197 2022-08-22 12:28:57.751742 cognitivefactory-interactive-clustering-gui-0.4.1/src/cognitivefactory/interactive_clustering_gui/__init__.py
+-rw-r--r--   0        0        0     1055 2022-08-26 11:33:58.069540 cognitivefactory-interactive-clustering-gui-0.4.1/src/cognitivefactory/interactive_clustering_gui/__main__.py
+-rw-r--r--   0        0        0   141835 2023-04-27 09:15:30.301653 cognitivefactory-interactive-clustering-gui-0.4.1/src/cognitivefactory/interactive_clustering_gui/app.py
+-rw-r--r--   0        0        0    34351 2023-02-16 17:35:42.446323 cognitivefactory-interactive-clustering-gui-0.4.1/src/cognitivefactory/interactive_clustering_gui/backgroundtasks.py
+-rw-r--r--   0        0        0     3495 2022-08-26 15:43:51.280254 cognitivefactory-interactive-clustering-gui-0.4.1/src/cognitivefactory/interactive_clustering_gui/cli.py
+-rw-r--r--   0        0        0     6527 2022-03-10 09:47:37.411388 cognitivefactory-interactive-clustering-gui-0.4.1/src/cognitivefactory/interactive_clustering_gui/css/new_styles.css
+-rw-r--r--   0        0        0    13550 2022-07-29 09:36:01.515330 cognitivefactory-interactive-clustering-gui-0.4.1/src/cognitivefactory/interactive_clustering_gui/css/styles.css
+-rw-r--r--   0        0        0     4433 2022-10-11 12:02:15.466779 cognitivefactory-interactive-clustering-gui-0.4.1/src/cognitivefactory/interactive_clustering_gui/html/_base.html
+-rw-r--r--   0        0        0    10046 2022-02-07 09:06:45.352415 cognitivefactory-interactive-clustering-gui-0.4.1/src/cognitivefactory/interactive_clustering_gui/html/analytics.html
+-rw-r--r--   0        0        0    19336 2023-04-27 09:14:46.100491 cognitivefactory-interactive-clustering-gui-0.4.1/src/cognitivefactory/interactive_clustering_gui/html/constraint_annotation.html
+-rw-r--r--   0        0        0    18182 2022-10-11 12:55:22.054343 cognitivefactory-interactive-clustering-gui-0.4.1/src/cognitivefactory/interactive_clustering_gui/html/constraints.html
+-rw-r--r--   0        0        0      635 2022-07-19 15:10:00.770489 cognitivefactory-interactive-clustering-gui-0.4.1/src/cognitivefactory/interactive_clustering_gui/html/error.html
+-rw-r--r--   0        0        0      600 2022-08-31 15:01:20.049462 cognitivefactory-interactive-clustering-gui-0.4.1/src/cognitivefactory/interactive_clustering_gui/html/help.html
+-rw-r--r--   0        0        0    15608 2022-08-31 14:59:25.146710 cognitivefactory-interactive-clustering-gui-0.4.1/src/cognitivefactory/interactive_clustering_gui/html/project_home.html
+-rw-r--r--   0        0        0     8971 2022-08-30 12:16:12.152401 cognitivefactory-interactive-clustering-gui-0.4.1/src/cognitivefactory/interactive_clustering_gui/html/projects_listing.html
+-rw-r--r--   0        0        0    35499 2022-07-26 11:22:40.014591 cognitivefactory-interactive-clustering-gui-0.4.1/src/cognitivefactory/interactive_clustering_gui/html/settings.html
+-rw-r--r--   0        0        0    13390 2022-10-11 12:56:56.367341 cognitivefactory-interactive-clustering-gui-0.4.1/src/cognitivefactory/interactive_clustering_gui/html/texts.html
+-rw-r--r--   0        0        0    14661 2022-06-03 12:53:45.394276 cognitivefactory-interactive-clustering-gui-0.4.1/src/cognitivefactory/interactive_clustering_gui/html/welcome.html
+-rw-r--r--   0        0        0     5561 2022-07-06 07:23:29.966040 cognitivefactory-interactive-clustering-gui-0.4.1/src/cognitivefactory/interactive_clustering_gui/js/analytics.js
+-rw-r--r--   0        0        0    17011 2022-07-07 11:36:32.036053 cognitivefactory-interactive-clustering-gui-0.4.1/src/cognitivefactory/interactive_clustering_gui/js/annotation.js
+-rw-r--r--   0        0        0     1133 2022-06-08 14:26:13.573749 cognitivefactory-interactive-clustering-gui-0.4.1/src/cognitivefactory/interactive_clustering_gui/js/collapsing.js
+-rw-r--r--   0        0        0    11925 2022-08-31 14:52:17.264788 cognitivefactory-interactive-clustering-gui-0.4.1/src/cognitivefactory/interactive_clustering_gui/js/constraints.js
+-rw-r--r--   0        0        0     3544 2022-08-31 14:50:40.593212 cognitivefactory-interactive-clustering-gui-0.4.1/src/cognitivefactory/interactive_clustering_gui/js/goto.js
+-rw-r--r--   0        0        0     3103 2022-07-07 06:56:56.317968 cognitivefactory-interactive-clustering-gui-0.4.1/src/cognitivefactory/interactive_clustering_gui/js/projects.js
+-rw-r--r--   0        0        0     8590 2022-07-29 09:12:47.093532 cognitivefactory-interactive-clustering-gui-0.4.1/src/cognitivefactory/interactive_clustering_gui/js/projects_listing.js
+-rw-r--r--   0        0        0    19918 2022-06-08 12:33:49.604197 cognitivefactory-interactive-clustering-gui-0.4.1/src/cognitivefactory/interactive_clustering_gui/js/settings.js
+-rw-r--r--   0        0        0    36228 2022-08-31 15:22:35.389593 cognitivefactory-interactive-clustering-gui-0.4.1/src/cognitivefactory/interactive_clustering_gui/js/status.js
+-rw-r--r--   0        0        0     7167 2022-06-24 15:41:20.664796 cognitivefactory-interactive-clustering-gui-0.4.1/src/cognitivefactory/interactive_clustering_gui/js/tasks.js
+-rw-r--r--   0        0        0      100 2022-07-21 16:16:51.353096 cognitivefactory-interactive-clustering-gui-0.4.1/src/cognitivefactory/interactive_clustering_gui/models/__init__.py
+-rw-r--r--   0        0        0     2090 2022-08-23 12:17:43.082363 cognitivefactory-interactive-clustering-gui-0.4.1/src/cognitivefactory/interactive_clustering_gui/models/queries.py
+-rw-r--r--   0        0        0    27380 2022-08-22 15:59:06.845649 cognitivefactory-interactive-clustering-gui-0.4.1/src/cognitivefactory/interactive_clustering_gui/models/settings.py
+-rw-r--r--   0        0        0    14411 2022-08-22 15:59:06.844652 cognitivefactory-interactive-clustering-gui-0.4.1/src/cognitivefactory/interactive_clustering_gui/models/states.py
+-rw-r--r--   0        0        0        0 2022-08-18 15:35:45.642146 cognitivefactory-interactive-clustering-gui-0.4.1/src/cognitivefactory/interactive_clustering_gui/py.typed
+-rw-r--r--   0        0        0    39169 2022-02-01 13:28:39.443263 cognitivefactory-interactive-clustering-gui-0.4.1/src/cognitivefactory/interactive_clustering_gui/resources/diagrams/example_clustering.png
+-rw-r--r--   0        0        0    25318 2022-02-01 13:32:14.299349 cognitivefactory-interactive-clustering-gui-0.4.1/src/cognitivefactory/interactive_clustering_gui/resources/diagrams/example_constrained_clustering.png
+-rw-r--r--   0        0        0    12842 2022-02-01 13:20:59.849702 cognitivefactory-interactive-clustering-gui-0.4.1/src/cognitivefactory/interactive_clustering_gui/resources/diagrams/example_constraints.png
+-rw-r--r--   0        0        0    10956 2022-02-03 08:57:31.044494 cognitivefactory-interactive-clustering-gui-0.4.1/src/cognitivefactory/interactive_clustering_gui/resources/diagrams/example_constraints_conflict.png
+-rw-r--r--   0        0        0    10672 2022-02-03 08:58:08.867236 cognitivefactory-interactive-clustering-gui-0.4.1/src/cognitivefactory/interactive_clustering_gui/resources/diagrams/example_constraints_inference_cannot_link.png
+-rw-r--r--   0        0        0     7018 2022-02-03 08:57:54.997255 cognitivefactory-interactive-clustering-gui-0.4.1/src/cognitivefactory/interactive_clustering_gui/resources/diagrams/example_constraints_inference_must_link.png
+-rw-r--r--   0        0        0    54984 2022-02-01 14:48:40.372500 cognitivefactory-interactive-clustering-gui-0.4.1/src/cognitivefactory/interactive_clustering_gui/resources/diagrams/example_sampling.png
+-rw-r--r--   0        0        0   196607 2022-02-01 17:32:29.088734 cognitivefactory-interactive-clustering-gui-0.4.1/src/cognitivefactory/interactive_clustering_gui/resources/diagrams/interactive_clustering.png
+-rw-r--r--   0        0        0    20973 2021-10-20 12:37:23.353701 cognitivefactory-interactive-clustering-gui-0.4.1/src/cognitivefactory/interactive_clustering_gui/resources/logos/github.png
+-rw-r--r--   0        0        0    12395 2022-07-06 08:49:07.035648 cognitivefactory-interactive-clustering-gui-0.4.1/src/cognitivefactory/interactive_clustering_gui/resources/logos/interactive_clustering_black.png
+-rw-r--r--   0        0        0     5648 2022-07-06 08:12:20.405379 cognitivefactory-interactive-clustering-gui-0.4.1/src/cognitivefactory/interactive_clustering_gui/resources/logos/interactive_clustering_blue.png
+-rw-r--r--   0        0        0     5645 2022-07-06 08:14:49.966463 cognitivefactory-interactive-clustering-gui-0.4.1/src/cognitivefactory/interactive_clustering_gui/resources/logos/interactive_clustering_gray_1.png
+-rw-r--r--   0        0        0     5415 2022-07-06 08:14:15.093499 cognitivefactory-interactive-clustering-gui-0.4.1/src/cognitivefactory/interactive_clustering_gui/resources/logos/interactive_clustering_gray_2.png
+-rw-r--r--   0        0        0    16485 2022-07-06 08:14:00.677811 cognitivefactory-interactive-clustering-gui-0.4.1/src/cognitivefactory/interactive_clustering_gui/resources/logos/interactive_clustering_pink.png
+-rw-r--r--   0        0        0    13258 2021-10-20 12:37:23.359688 cognitivefactory-interactive-clustering-gui-0.4.1/src/cognitivefactory/interactive_clustering_gui/resources/logos/interactive_clustering_white.png
+-rw-r--r--   0        0        0      196 2022-08-22 15:59:06.825664 cognitivefactory-interactive-clustering-gui-0.4.1/tests/__init__.py
+-rw-r--r--   0        0        0     3249 2022-08-26 14:31:56.269726 cognitivefactory-interactive-clustering-gui-0.4.1/tests/conftest.py
+-rw-r--r--   0        0        0        2 2022-07-11 12:07:21.312463 cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/0a_INITIALIZATION_WITHOUT_MODELIZATION/clustering.json
+-rw-r--r--   0        0        0        2 2022-07-11 12:07:21.271572 cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/0a_INITIALIZATION_WITHOUT_MODELIZATION/constraints.json
+-rw-r--r--   0        0        0      144 2022-07-11 12:24:22.394714 cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/0a_INITIALIZATION_WITHOUT_MODELIZATION/metadata.json
+-rw-r--r--   0        0        0     3045 2022-07-11 12:07:21.303486 cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/0a_INITIALIZATION_WITHOUT_MODELIZATION/modelization.json
+-rw-r--r--   0        0        0        2 2022-07-11 12:07:21.309471 cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/0a_INITIALIZATION_WITHOUT_MODELIZATION/sampling.json
+-rw-r--r--   0        0        0      696 2022-07-11 12:13:45.311609 cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/0a_INITIALIZATION_WITHOUT_MODELIZATION/settings.json
+-rw-r--r--   0        0        0       99 2022-07-11 12:07:21.264592 cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/0a_INITIALIZATION_WITHOUT_MODELIZATION/status.json
+-rw-r--r--   0        0        0     6659 2022-07-11 12:07:21.267583 cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/0a_INITIALIZATION_WITHOUT_MODELIZATION/texts.json
+-rw-r--r--   0        0        0        2 2022-07-11 12:07:21.312463 cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/0b_INITIALIZATION_WITH_PENDING_MODELIZATION/clustering.json
+-rw-r--r--   0        0        0        2 2022-07-11 12:07:21.271572 cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/0b_INITIALIZATION_WITH_PENDING_MODELIZATION/constraints.json
+-rw-r--r--   0        0        0      149 2022-07-25 14:28:29.853559 cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/0b_INITIALIZATION_WITH_PENDING_MODELIZATION/metadata.json
+-rw-r--r--   0        0        0     3045 2022-07-11 12:07:21.303486 cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/0b_INITIALIZATION_WITH_PENDING_MODELIZATION/modelization.json
+-rw-r--r--   0        0        0        2 2022-07-11 12:07:21.309471 cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/0b_INITIALIZATION_WITH_PENDING_MODELIZATION/sampling.json
+-rw-r--r--   0        0        0      696 2022-07-11 12:13:45.311609 cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/0b_INITIALIZATION_WITH_PENDING_MODELIZATION/settings.json
+-rw-r--r--   0        0        0      198 2022-08-23 08:03:11.312599 cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/0b_INITIALIZATION_WITH_PENDING_MODELIZATION/status.json
+-rw-r--r--   0        0        0     6659 2022-07-11 12:07:21.267583 cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/0b_INITIALIZATION_WITH_PENDING_MODELIZATION/texts.json
+-rw-r--r--   0        0        0        2 2022-07-11 12:07:21.312463 cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/0c_INITIALIZATION_WITH_WORKING_MODELIZATION/clustering.json
+-rw-r--r--   0        0        0        2 2022-07-11 12:07:21.271572 cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/0c_INITIALIZATION_WITH_WORKING_MODELIZATION/constraints.json
+-rw-r--r--   0        0        0      149 2022-07-25 14:29:48.166071 cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/0c_INITIALIZATION_WITH_WORKING_MODELIZATION/metadata.json
+-rw-r--r--   0        0        0     3045 2022-07-11 12:07:21.303486 cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/0c_INITIALIZATION_WITH_WORKING_MODELIZATION/modelization.json
+-rw-r--r--   0        0        0        2 2022-07-11 12:07:21.309471 cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/0c_INITIALIZATION_WITH_WORKING_MODELIZATION/sampling.json
+-rw-r--r--   0        0        0      696 2022-07-11 12:13:45.311609 cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/0c_INITIALIZATION_WITH_WORKING_MODELIZATION/settings.json
+-rw-r--r--   0        0        0      175 2022-08-23 08:03:11.377428 cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/0c_INITIALIZATION_WITH_WORKING_MODELIZATION/status.json
+-rw-r--r--   0        0        0     6659 2022-07-11 12:07:21.267583 cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/0c_INITIALIZATION_WITH_WORKING_MODELIZATION/texts.json
+-rw-r--r--   0        0        0        2 2022-07-11 12:07:21.312463 cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/0d_CLUSTERING_TODO/clustering.json
+-rw-r--r--   0        0        0        2 2022-07-11 12:10:27.067191 cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/0d_CLUSTERING_TODO/constraints.json
+-rw-r--r--   0        0        0     1880 2022-08-23 13:18:44.586771 cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/0d_CLUSTERING_TODO/constraints_manager.pkl
+-rw-r--r--   0        0        0      124 2022-07-25 14:32:47.239376 cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/0d_CLUSTERING_TODO/metadata.json
+-rw-r--r--   0        0        0     3045 2022-07-11 12:10:27.509082 cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/0d_CLUSTERING_TODO/modelization.json
+-rw-r--r--   0        0        0        2 2022-07-11 12:07:21.309471 cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/0d_CLUSTERING_TODO/sampling.json
+-rw-r--r--   0        0        0      696 2022-07-11 12:13:54.079094 cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/0d_CLUSTERING_TODO/settings.json
+-rw-r--r--   0        0        0       79 2022-07-11 12:10:27.524042 cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/0d_CLUSTERING_TODO/status.json
+-rw-r--r--   0        0        0     6513 2022-07-11 12:10:23.869094 cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/0d_CLUSTERING_TODO/texts.json
+-rw-r--r--   0        0        0     5825 2022-07-11 12:10:24.327037 cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/0d_CLUSTERING_TODO/vectors.pkl
+-rw-r--r--   0        0        0     2106 2022-07-11 12:10:25.284783 cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/0d_CLUSTERING_TODO/vectors_2D.json
+-rw-r--r--   0        0        0     2904 2022-07-11 12:10:26.615845 cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/0d_CLUSTERING_TODO/vectors_3D.json
+-rw-r--r--   0        0        0        2 2022-07-11 12:07:21.312463 cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/0e_CLUSTERING_PENDING/clustering.json
+-rw-r--r--   0        0        0        2 2022-07-11 12:10:27.067191 cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/0e_CLUSTERING_PENDING/constraints.json
+-rw-r--r--   0        0        0     1880 2022-08-23 13:18:41.974764 cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/0e_CLUSTERING_PENDING/constraints_manager.pkl
+-rw-r--r--   0        0        0      127 2022-07-25 14:31:40.122180 cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/0e_CLUSTERING_PENDING/metadata.json
+-rw-r--r--   0        0        0     3045 2022-07-11 12:10:27.509082 cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/0e_CLUSTERING_PENDING/modelization.json
+-rw-r--r--   0        0        0        2 2022-07-11 12:07:21.309471 cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/0e_CLUSTERING_PENDING/sampling.json
+-rw-r--r--   0        0        0      696 2022-07-11 12:13:34.463283 cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/0e_CLUSTERING_PENDING/settings.json
+-rw-r--r--   0        0        0      177 2022-08-23 08:03:11.373438 cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/0e_CLUSTERING_PENDING/status.json
+-rw-r--r--   0        0        0     6513 2022-07-11 12:10:23.869094 cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/0e_CLUSTERING_PENDING/texts.json
+-rw-r--r--   0        0        0     5825 2022-07-11 12:10:24.327037 cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/0e_CLUSTERING_PENDING/vectors.pkl
+-rw-r--r--   0        0        0     2106 2022-07-11 12:10:25.284783 cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/0e_CLUSTERING_PENDING/vectors_2D.json
+-rw-r--r--   0        0        0     2904 2022-07-11 12:10:26.615845 cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/0e_CLUSTERING_PENDING/vectors_3D.json
+-rw-r--r--   0        0        0        2 2022-07-11 12:07:21.312463 cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/0f_CLUSTERING_WORKING/clustering.json
+-rw-r--r--   0        0        0        2 2022-07-11 12:10:27.067191 cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/0f_CLUSTERING_WORKING/constraints.json
+-rw-r--r--   0        0        0     1880 2022-08-23 13:18:41.982747 cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/0f_CLUSTERING_WORKING/constraints_manager.pkl
+-rw-r--r--   0        0        0      127 2022-07-25 14:34:10.768459 cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/0f_CLUSTERING_WORKING/metadata.json
+-rw-r--r--   0        0        0     3045 2022-07-11 12:10:27.509082 cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/0f_CLUSTERING_WORKING/modelization.json
+-rw-r--r--   0        0        0        2 2022-07-11 12:07:21.309471 cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/0f_CLUSTERING_WORKING/sampling.json
+-rw-r--r--   0        0        0      696 2022-07-11 12:13:34.463283 cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/0f_CLUSTERING_WORKING/settings.json
+-rw-r--r--   0        0        0      149 2022-08-23 08:03:11.366457 cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/0f_CLUSTERING_WORKING/status.json
+-rw-r--r--   0        0        0     6513 2022-07-11 12:10:23.869094 cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/0f_CLUSTERING_WORKING/texts.json
+-rw-r--r--   0        0        0     5825 2022-07-11 12:10:24.327037 cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/0f_CLUSTERING_WORKING/vectors.pkl
+-rw-r--r--   0        0        0     2106 2022-07-11 12:10:25.284783 cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/0f_CLUSTERING_WORKING/vectors_2D.json
+-rw-r--r--   0        0        0     2904 2022-07-11 12:10:26.615845 cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/0f_CLUSTERING_WORKING/vectors_3D.json
+-rw-r--r--   0        0        0      444 2022-07-11 12:14:11.348217 cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/0g_ITERATION_END/clustering.json
+-rw-r--r--   0        0        0        2 2022-07-11 12:10:27.067191 cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/0g_ITERATION_END/constraints.json
+-rw-r--r--   0        0        0     1880 2022-08-23 13:18:41.988728 cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/0g_ITERATION_END/constraints_manager.pkl
+-rw-r--r--   0        0        0      122 2022-07-25 14:34:47.905746 cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/0g_ITERATION_END/metadata.json
+-rw-r--r--   0        0        0     3045 2022-07-11 12:10:27.509082 cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/0g_ITERATION_END/modelization.json
+-rw-r--r--   0        0        0        2 2022-07-11 12:07:21.309471 cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/0g_ITERATION_END/sampling.json
+-rw-r--r--   0        0        0      696 2022-07-11 12:13:34.463283 cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/0g_ITERATION_END/settings.json
+-rw-r--r--   0        0        0       77 2022-07-11 12:14:11.366169 cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/0g_ITERATION_END/status.json
+-rw-r--r--   0        0        0     6513 2022-07-11 12:10:23.869094 cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/0g_ITERATION_END/texts.json
+-rw-r--r--   0        0        0     5825 2022-07-11 12:10:24.327037 cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/0g_ITERATION_END/vectors.pkl
+-rw-r--r--   0        0        0     2106 2022-07-11 12:10:25.284783 cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/0g_ITERATION_END/vectors_2D.json
+-rw-r--r--   0        0        0     2904 2022-07-11 12:10:26.615845 cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/0g_ITERATION_END/vectors_3D.json
+-rw-r--r--   0        0        0      444 2022-07-11 12:14:11.348217 cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/1a_SAMPLING_TODO/clustering.json
+-rw-r--r--   0        0        0        2 2022-07-11 12:10:27.067191 cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/1a_SAMPLING_TODO/constraints.json
+-rw-r--r--   0        0        0     1880 2022-08-23 13:18:41.994713 cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/1a_SAMPLING_TODO/constraints_manager.pkl
+-rw-r--r--   0        0        0      122 2022-07-11 12:26:59.431426 cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/1a_SAMPLING_TODO/metadata.json
+-rw-r--r--   0        0        0     3045 2022-07-11 12:10:27.509082 cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/1a_SAMPLING_TODO/modelization.json
+-rw-r--r--   0        0        0        2 2022-07-11 12:07:21.309471 cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/1a_SAMPLING_TODO/sampling.json
+-rw-r--r--   0        0        0     1580 2022-07-11 12:18:44.031863 cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/1a_SAMPLING_TODO/settings.json
+-rw-r--r--   0        0        0       77 2022-07-11 12:18:44.033857 cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/1a_SAMPLING_TODO/status.json
+-rw-r--r--   0        0        0     6513 2022-07-11 12:10:23.869094 cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/1a_SAMPLING_TODO/texts.json
+-rw-r--r--   0        0        0     5825 2022-07-11 12:10:24.327037 cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/1a_SAMPLING_TODO/vectors.pkl
+-rw-r--r--   0        0        0     2106 2022-07-11 12:10:25.284783 cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/1a_SAMPLING_TODO/vectors_2D.json
+-rw-r--r--   0        0        0     2904 2022-07-11 12:10:26.615845 cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/1a_SAMPLING_TODO/vectors_3D.json
+-rw-r--r--   0        0        0      444 2022-07-11 12:14:11.348217 cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/1b_SAMPLING_PENDING/clustering.json
+-rw-r--r--   0        0        0        2 2022-07-11 12:10:27.067191 cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/1b_SAMPLING_PENDING/constraints.json
+-rw-r--r--   0        0        0     1880 2022-08-23 13:18:42.002693 cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/1b_SAMPLING_PENDING/constraints_manager.pkl
+-rw-r--r--   0        0        0      125 2022-07-11 12:27:05.724791 cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/1b_SAMPLING_PENDING/metadata.json
+-rw-r--r--   0        0        0     3045 2022-07-11 12:10:27.509082 cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/1b_SAMPLING_PENDING/modelization.json
+-rw-r--r--   0        0        0        2 2022-07-11 12:07:21.309471 cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/1b_SAMPLING_PENDING/sampling.json
+-rw-r--r--   0        0        0     1580 2022-07-11 12:18:44.031863 cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/1b_SAMPLING_PENDING/settings.json
+-rw-r--r--   0        0        0      174 2022-08-23 08:03:11.372441 cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/1b_SAMPLING_PENDING/status.json
+-rw-r--r--   0        0        0     6513 2022-07-11 12:10:23.869094 cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/1b_SAMPLING_PENDING/texts.json
+-rw-r--r--   0        0        0     5825 2022-07-11 12:10:24.327037 cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/1b_SAMPLING_PENDING/vectors.pkl
+-rw-r--r--   0        0        0     2106 2022-07-11 12:10:25.284783 cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/1b_SAMPLING_PENDING/vectors_2D.json
+-rw-r--r--   0        0        0     2904 2022-07-11 12:10:26.615845 cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/1b_SAMPLING_PENDING/vectors_3D.json
+-rw-r--r--   0        0        0      444 2022-07-11 12:14:11.348217 cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/1c_SAMPLING_WORKING/clustering.json
+-rw-r--r--   0        0        0        2 2022-07-11 12:10:27.067191 cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/1c_SAMPLING_WORKING/constraints.json
+-rw-r--r--   0        0        0     1880 2022-08-23 13:18:42.008677 cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/1c_SAMPLING_WORKING/constraints_manager.pkl
+-rw-r--r--   0        0        0      125 2022-07-11 12:27:12.700825 cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/1c_SAMPLING_WORKING/metadata.json
+-rw-r--r--   0        0        0     3045 2022-07-11 12:10:27.509082 cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/1c_SAMPLING_WORKING/modelization.json
+-rw-r--r--   0        0        0        2 2022-07-11 12:07:21.309471 cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/1c_SAMPLING_WORKING/sampling.json
+-rw-r--r--   0        0        0     1580 2022-07-11 12:18:44.031863 cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/1c_SAMPLING_WORKING/settings.json
+-rw-r--r--   0        0        0      167 2022-08-23 08:03:11.366457 cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/1c_SAMPLING_WORKING/status.json
+-rw-r--r--   0        0        0     6513 2022-07-11 12:10:23.869094 cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/1c_SAMPLING_WORKING/texts.json
+-rw-r--r--   0        0        0     5825 2022-07-11 12:10:24.327037 cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/1c_SAMPLING_WORKING/vectors.pkl
+-rw-r--r--   0        0        0     2106 2022-07-11 12:10:25.284783 cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/1c_SAMPLING_WORKING/vectors_2D.json
+-rw-r--r--   0        0        0     2904 2022-07-11 12:10:26.615845 cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/1c_SAMPLING_WORKING/vectors_3D.json
+-rw-r--r--   0        0        0      444 2022-07-11 12:14:11.348217 cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/1d_ANNOTATION_WITH_UPTODATE_MODELIZATION/clustering.json
+-rw-r--r--   0        0        0     9980 2022-07-11 12:20:33.453660 cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/1d_ANNOTATION_WITH_UPTODATE_MODELIZATION/constraints.json
+-rw-r--r--   0        0        0     1880 2022-08-23 13:18:42.015672 cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/1d_ANNOTATION_WITH_UPTODATE_MODELIZATION/constraints_manager.pkl
+-rw-r--r--   0        0        0      146 2022-07-11 12:27:29.714251 cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/1d_ANNOTATION_WITH_UPTODATE_MODELIZATION/metadata.json
+-rw-r--r--   0        0        0     3045 2022-07-11 12:10:27.509082 cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/1d_ANNOTATION_WITH_UPTODATE_MODELIZATION/modelization.json
+-rw-r--r--   0        0        0      498 2022-07-11 12:20:33.448671 cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/1d_ANNOTATION_WITH_UPTODATE_MODELIZATION/sampling.json
+-rw-r--r--   0        0        0     1580 2022-07-11 12:18:44.031863 cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/1d_ANNOTATION_WITH_UPTODATE_MODELIZATION/settings.json
+-rw-r--r--   0        0        0      101 2022-07-11 12:20:33.494108 cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/1d_ANNOTATION_WITH_UPTODATE_MODELIZATION/status.json
+-rw-r--r--   0        0        0     6513 2022-07-11 12:10:23.869094 cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/1d_ANNOTATION_WITH_UPTODATE_MODELIZATION/texts.json
+-rw-r--r--   0        0        0     5825 2022-07-11 12:10:24.327037 cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/1d_ANNOTATION_WITH_UPTODATE_MODELIZATION/vectors.pkl
+-rw-r--r--   0        0        0     2106 2022-07-11 12:10:25.284783 cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/1d_ANNOTATION_WITH_UPTODATE_MODELIZATION/vectors_2D.json
+-rw-r--r--   0        0        0     2904 2022-07-11 12:10:26.615845 cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/1d_ANNOTATION_WITH_UPTODATE_MODELIZATION/vectors_3D.json
+-rw-r--r--   0        0        0      444 2022-07-11 12:14:11.348217 cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/1e_ANNOTATION_WITH_OUTDATED_MODELIZATION_WITHOUT_CONFLICTS/clustering.json
+-rw-r--r--   0        0        0    11371 2022-07-11 13:20:21.670315 cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/1e_ANNOTATION_WITH_OUTDATED_MODELIZATION_WITHOUT_CONFLICTS/constraints.json
+-rw-r--r--   0        0        0     2160 2022-08-23 13:18:42.021642 cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/1e_ANNOTATION_WITH_OUTDATED_MODELIZATION_WITHOUT_CONFLICTS/constraints_manager.pkl
+-rw-r--r--   0        0        0      164 2022-07-11 13:26:02.683020 cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/1e_ANNOTATION_WITH_OUTDATED_MODELIZATION_WITHOUT_CONFLICTS/metadata.json
+-rw-r--r--   0        0        0     3045 2022-07-11 13:21:08.841360 cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/1e_ANNOTATION_WITH_OUTDATED_MODELIZATION_WITHOUT_CONFLICTS/modelization.json
+-rw-r--r--   0        0        0      498 2022-07-11 12:20:33.448671 cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/1e_ANNOTATION_WITH_OUTDATED_MODELIZATION_WITHOUT_CONFLICTS/sampling.json
+-rw-r--r--   0        0        0     1580 2022-07-11 12:18:44.031863 cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/1e_ANNOTATION_WITH_OUTDATED_MODELIZATION_WITHOUT_CONFLICTS/settings.json
+-rw-r--r--   0        0        0      119 2022-07-11 13:19:13.465236 cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/1e_ANNOTATION_WITH_OUTDATED_MODELIZATION_WITHOUT_CONFLICTS/status.json
+-rw-r--r--   0        0        0     6512 2022-07-11 13:18:08.188828 cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/1e_ANNOTATION_WITH_OUTDATED_MODELIZATION_WITHOUT_CONFLICTS/texts.json
+-rw-r--r--   0        0        0     5469 2022-07-11 13:18:08.637543 cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/1e_ANNOTATION_WITH_OUTDATED_MODELIZATION_WITHOUT_CONFLICTS/vectors.pkl
+-rw-r--r--   0        0        0     2001 2022-07-11 13:18:09.816595 cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/1e_ANNOTATION_WITH_OUTDATED_MODELIZATION_WITHOUT_CONFLICTS/vectors_2D.json
+-rw-r--r--   0        0        0     2773 2022-07-11 13:18:10.735536 cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/1e_ANNOTATION_WITH_OUTDATED_MODELIZATION_WITHOUT_CONFLICTS/vectors_3D.json
+-rw-r--r--   0        0        0      444 2022-07-11 12:14:11.348217 cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/1f_ANNOTATION_WITH_PENDING_MODELIZATION_WITHOUT_CONFLICTS/clustering.json
+-rw-r--r--   0        0        0    11371 2022-07-11 13:20:21.670315 cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/1f_ANNOTATION_WITH_PENDING_MODELIZATION_WITHOUT_CONFLICTS/constraints.json
+-rw-r--r--   0        0        0     2160 2022-08-23 13:18:42.028634 cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/1f_ANNOTATION_WITH_PENDING_MODELIZATION_WITHOUT_CONFLICTS/constraints_manager.pkl
+-rw-r--r--   0        0        0      163 2022-07-11 13:24:30.805153 cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/1f_ANNOTATION_WITH_PENDING_MODELIZATION_WITHOUT_CONFLICTS/metadata.json
+-rw-r--r--   0        0        0     3045 2022-07-11 13:21:08.841360 cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/1f_ANNOTATION_WITH_PENDING_MODELIZATION_WITHOUT_CONFLICTS/modelization.json
+-rw-r--r--   0        0        0      498 2022-07-11 12:20:33.448671 cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/1f_ANNOTATION_WITH_PENDING_MODELIZATION_WITHOUT_CONFLICTS/sampling.json
+-rw-r--r--   0        0        0     1580 2022-07-11 12:18:44.031863 cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/1f_ANNOTATION_WITH_PENDING_MODELIZATION_WITHOUT_CONFLICTS/settings.json
+-rw-r--r--   0        0        0      212 2022-08-23 08:03:11.366457 cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/1f_ANNOTATION_WITH_PENDING_MODELIZATION_WITHOUT_CONFLICTS/status.json
+-rw-r--r--   0        0        0     6512 2022-07-11 13:18:08.188828 cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/1f_ANNOTATION_WITH_PENDING_MODELIZATION_WITHOUT_CONFLICTS/texts.json
+-rw-r--r--   0        0        0     5469 2022-07-11 13:18:08.637543 cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/1f_ANNOTATION_WITH_PENDING_MODELIZATION_WITHOUT_CONFLICTS/vectors.pkl
+-rw-r--r--   0        0        0     2001 2022-07-11 13:18:09.816595 cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/1f_ANNOTATION_WITH_PENDING_MODELIZATION_WITHOUT_CONFLICTS/vectors_2D.json
+-rw-r--r--   0        0        0     2773 2022-07-11 13:18:10.735536 cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/1f_ANNOTATION_WITH_PENDING_MODELIZATION_WITHOUT_CONFLICTS/vectors_3D.json
+-rw-r--r--   0        0        0      444 2022-07-11 12:14:11.348217 cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/1g_ANNOTATION_WITH_WORKING_MODELIZATION_WITHOUT_CONFLICTS/clustering.json
+-rw-r--r--   0        0        0    11371 2022-07-11 13:20:21.670315 cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/1g_ANNOTATION_WITH_WORKING_MODELIZATION_WITHOUT_CONFLICTS/constraints.json
+-rw-r--r--   0        0        0     2160 2022-08-23 13:18:42.035605 cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/1g_ANNOTATION_WITH_WORKING_MODELIZATION_WITHOUT_CONFLICTS/constraints_manager.pkl
+-rw-r--r--   0        0        0      163 2022-07-11 13:23:55.651507 cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/1g_ANNOTATION_WITH_WORKING_MODELIZATION_WITHOUT_CONFLICTS/metadata.json
+-rw-r--r--   0        0        0     3045 2022-07-11 13:21:08.841360 cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/1g_ANNOTATION_WITH_WORKING_MODELIZATION_WITHOUT_CONFLICTS/modelization.json
+-rw-r--r--   0        0        0      498 2022-07-11 12:20:33.448671 cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/1g_ANNOTATION_WITH_WORKING_MODELIZATION_WITHOUT_CONFLICTS/sampling.json
+-rw-r--r--   0        0        0     1580 2022-07-11 12:18:44.031863 cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/1g_ANNOTATION_WITH_WORKING_MODELIZATION_WITHOUT_CONFLICTS/settings.json
+-rw-r--r--   0        0        0      189 2022-08-23 08:03:11.362489 cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/1g_ANNOTATION_WITH_WORKING_MODELIZATION_WITHOUT_CONFLICTS/status.json
+-rw-r--r--   0        0        0     6512 2022-07-11 13:18:08.188828 cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/1g_ANNOTATION_WITH_WORKING_MODELIZATION_WITHOUT_CONFLICTS/texts.json
+-rw-r--r--   0        0        0     5469 2022-07-11 13:18:08.637543 cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/1g_ANNOTATION_WITH_WORKING_MODELIZATION_WITHOUT_CONFLICTS/vectors.pkl
+-rw-r--r--   0        0        0     2001 2022-07-11 13:18:09.816595 cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/1g_ANNOTATION_WITH_WORKING_MODELIZATION_WITHOUT_CONFLICTS/vectors_2D.json
+-rw-r--r--   0        0        0     2773 2022-07-11 13:18:10.735536 cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/1g_ANNOTATION_WITH_WORKING_MODELIZATION_WITHOUT_CONFLICTS/vectors_3D.json
+-rw-r--r--   0        0        0      444 2022-07-11 12:14:11.348217 cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/1h_ANNOTATION_WITH_OUTDATED_MODELIZATION_WITH_CONFLICTS/clustering.json
+-rw-r--r--   0        0        0    11370 2022-07-11 13:21:59.471239 cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/1h_ANNOTATION_WITH_OUTDATED_MODELIZATION_WITH_CONFLICTS/constraints.json
+-rw-r--r--   0        0        0     2169 2022-08-23 13:18:42.042584 cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/1h_ANNOTATION_WITH_OUTDATED_MODELIZATION_WITH_CONFLICTS/constraints_manager.pkl
+-rw-r--r--   0        0        0      161 2022-07-11 13:23:30.838275 cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/1h_ANNOTATION_WITH_OUTDATED_MODELIZATION_WITH_CONFLICTS/metadata.json
+-rw-r--r--   0        0        0     7327 2022-07-11 13:21:59.906137 cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/1h_ANNOTATION_WITH_OUTDATED_MODELIZATION_WITH_CONFLICTS/modelization.json
+-rw-r--r--   0        0        0      498 2022-07-11 12:20:33.448671 cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/1h_ANNOTATION_WITH_OUTDATED_MODELIZATION_WITH_CONFLICTS/sampling.json
+-rw-r--r--   0        0        0     1580 2022-07-11 12:18:44.031863 cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/1h_ANNOTATION_WITH_OUTDATED_MODELIZATION_WITH_CONFLICTS/settings.json
+-rw-r--r--   0        0        0      116 2022-07-11 13:21:59.916111 cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/1h_ANNOTATION_WITH_OUTDATED_MODELIZATION_WITH_CONFLICTS/status.json
+-rw-r--r--   0        0        0     6512 2022-07-11 13:21:55.273853 cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/1h_ANNOTATION_WITH_OUTDATED_MODELIZATION_WITH_CONFLICTS/texts.json
+-rw-r--r--   0        0        0     5469 2022-07-11 13:21:55.838885 cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/1h_ANNOTATION_WITH_OUTDATED_MODELIZATION_WITH_CONFLICTS/vectors.pkl
+-rw-r--r--   0        0        0     2001 2022-07-11 13:21:57.677538 cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/1h_ANNOTATION_WITH_OUTDATED_MODELIZATION_WITH_CONFLICTS/vectors_2D.json
+-rw-r--r--   0        0        0     2773 2022-07-11 13:21:59.020204 cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/1h_ANNOTATION_WITH_OUTDATED_MODELIZATION_WITH_CONFLICTS/vectors_3D.json
+-rw-r--r--   0        0        0      444 2022-07-11 12:14:11.348217 cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/1i_ANNOTATION_WITH_OUTDATED_MODELIZATION_WITH_CONFLICTS/clustering.json
+-rw-r--r--   0        0        0    11443 2022-07-11 13:30:14.546184 cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/1i_ANNOTATION_WITH_OUTDATED_MODELIZATION_WITH_CONFLICTS/constraints.json
+-rw-r--r--   0        0        0     2169 2022-08-23 13:18:42.048571 cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/1i_ANNOTATION_WITH_OUTDATED_MODELIZATION_WITH_CONFLICTS/constraints_manager.pkl
+-rw-r--r--   0        0        0      161 2022-07-11 13:28:17.222075 cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/1i_ANNOTATION_WITH_OUTDATED_MODELIZATION_WITH_CONFLICTS/metadata.json
+-rw-r--r--   0        0        0     7327 2022-07-11 13:29:05.933834 cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/1i_ANNOTATION_WITH_OUTDATED_MODELIZATION_WITH_CONFLICTS/modelization.json
+-rw-r--r--   0        0        0      498 2022-07-11 12:20:33.448671 cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/1i_ANNOTATION_WITH_OUTDATED_MODELIZATION_WITH_CONFLICTS/sampling.json
+-rw-r--r--   0        0        0     1580 2022-07-11 12:18:44.031863 cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/1i_ANNOTATION_WITH_OUTDATED_MODELIZATION_WITH_CONFLICTS/settings.json
+-rw-r--r--   0        0        0      116 2022-07-11 13:30:14.540199 cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/1i_ANNOTATION_WITH_OUTDATED_MODELIZATION_WITH_CONFLICTS/status.json
+-rw-r--r--   0        0        0     6512 2022-07-11 13:29:02.736926 cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/1i_ANNOTATION_WITH_OUTDATED_MODELIZATION_WITH_CONFLICTS/texts.json
+-rw-r--r--   0        0        0     5469 2022-07-11 13:29:03.209019 cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/1i_ANNOTATION_WITH_OUTDATED_MODELIZATION_WITH_CONFLICTS/vectors.pkl
+-rw-r--r--   0        0        0     2001 2022-07-11 13:29:04.093840 cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/1i_ANNOTATION_WITH_OUTDATED_MODELIZATION_WITH_CONFLICTS/vectors_2D.json
+-rw-r--r--   0        0        0     2773 2022-07-11 13:29:05.015142 cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/1i_ANNOTATION_WITH_OUTDATED_MODELIZATION_WITH_CONFLICTS/vectors_3D.json
+-rw-r--r--   0        0        0      444 2022-07-11 12:14:11.348217 cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/1j_ANNOTATION_WITH_PENDING_MODELIZATION_WITH_CONFLICTS/clustering.json
+-rw-r--r--   0        0        0    11443 2022-07-11 13:30:14.546184 cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/1j_ANNOTATION_WITH_PENDING_MODELIZATION_WITH_CONFLICTS/constraints.json
+-rw-r--r--   0        0        0     2169 2022-08-23 13:18:42.054553 cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/1j_ANNOTATION_WITH_PENDING_MODELIZATION_WITH_CONFLICTS/constraints_manager.pkl
+-rw-r--r--   0        0        0      160 2022-07-11 13:33:48.143189 cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/1j_ANNOTATION_WITH_PENDING_MODELIZATION_WITH_CONFLICTS/metadata.json
+-rw-r--r--   0        0        0     7327 2022-07-11 13:29:05.933834 cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/1j_ANNOTATION_WITH_PENDING_MODELIZATION_WITH_CONFLICTS/modelization.json
+-rw-r--r--   0        0        0      498 2022-07-11 12:20:33.448671 cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/1j_ANNOTATION_WITH_PENDING_MODELIZATION_WITH_CONFLICTS/sampling.json
+-rw-r--r--   0        0        0     1580 2022-07-11 12:18:44.031863 cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/1j_ANNOTATION_WITH_PENDING_MODELIZATION_WITH_CONFLICTS/settings.json
+-rw-r--r--   0        0        0      209 2022-08-23 08:03:11.358480 cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/1j_ANNOTATION_WITH_PENDING_MODELIZATION_WITH_CONFLICTS/status.json
+-rw-r--r--   0        0        0     6512 2022-07-11 13:29:02.736926 cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/1j_ANNOTATION_WITH_PENDING_MODELIZATION_WITH_CONFLICTS/texts.json
+-rw-r--r--   0        0        0     5469 2022-07-11 13:29:03.209019 cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/1j_ANNOTATION_WITH_PENDING_MODELIZATION_WITH_CONFLICTS/vectors.pkl
+-rw-r--r--   0        0        0     2001 2022-07-11 13:29:04.093840 cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/1j_ANNOTATION_WITH_PENDING_MODELIZATION_WITH_CONFLICTS/vectors_2D.json
+-rw-r--r--   0        0        0     2773 2022-07-11 13:29:05.015142 cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/1j_ANNOTATION_WITH_PENDING_MODELIZATION_WITH_CONFLICTS/vectors_3D.json
+-rw-r--r--   0        0        0      444 2022-07-11 12:14:11.348217 cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/1k_ANNOTATION_WITH_WORKING_MODELIZATION_WITH_CONFLICTS/clustering.json
+-rw-r--r--   0        0        0    11443 2022-07-11 13:30:14.546184 cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/1k_ANNOTATION_WITH_WORKING_MODELIZATION_WITH_CONFLICTS/constraints.json
+-rw-r--r--   0        0        0     2169 2022-08-23 13:18:42.061533 cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/1k_ANNOTATION_WITH_WORKING_MODELIZATION_WITH_CONFLICTS/constraints_manager.pkl
+-rw-r--r--   0        0        0      160 2022-07-11 13:32:51.404211 cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/1k_ANNOTATION_WITH_WORKING_MODELIZATION_WITH_CONFLICTS/metadata.json
+-rw-r--r--   0        0        0     7327 2022-07-11 13:29:05.933834 cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/1k_ANNOTATION_WITH_WORKING_MODELIZATION_WITH_CONFLICTS/modelization.json
+-rw-r--r--   0        0        0      498 2022-07-11 12:20:33.448671 cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/1k_ANNOTATION_WITH_WORKING_MODELIZATION_WITH_CONFLICTS/sampling.json
+-rw-r--r--   0        0        0     1580 2022-07-11 12:18:44.031863 cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/1k_ANNOTATION_WITH_WORKING_MODELIZATION_WITH_CONFLICTS/settings.json
+-rw-r--r--   0        0        0      186 2022-08-23 08:03:11.358480 cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/1k_ANNOTATION_WITH_WORKING_MODELIZATION_WITH_CONFLICTS/status.json
+-rw-r--r--   0        0        0     6512 2022-07-11 13:29:02.736926 cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/1k_ANNOTATION_WITH_WORKING_MODELIZATION_WITH_CONFLICTS/texts.json
+-rw-r--r--   0        0        0     5469 2022-07-11 13:29:03.209019 cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/1k_ANNOTATION_WITH_WORKING_MODELIZATION_WITH_CONFLICTS/vectors.pkl
+-rw-r--r--   0        0        0     2001 2022-07-11 13:29:04.093840 cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/1k_ANNOTATION_WITH_WORKING_MODELIZATION_WITH_CONFLICTS/vectors_2D.json
+-rw-r--r--   0        0        0     2773 2022-07-11 13:29:05.015142 cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/1k_ANNOTATION_WITH_WORKING_MODELIZATION_WITH_CONFLICTS/vectors_3D.json
+-rw-r--r--   0        0        0      444 2022-07-11 12:14:11.348217 cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/1l_ANNOTATION_WITH_UPTODATE_MODELIZATION/clustering.json
+-rw-r--r--   0        0        0    11444 2022-07-11 13:32:13.084020 cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/1l_ANNOTATION_WITH_UPTODATE_MODELIZATION/constraints.json
+-rw-r--r--   0        0        0     2160 2022-08-23 13:18:42.067517 cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/1l_ANNOTATION_WITH_UPTODATE_MODELIZATION/constraints_manager.pkl
+-rw-r--r--   0        0        0      146 2022-07-11 13:35:34.340671 cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/1l_ANNOTATION_WITH_UPTODATE_MODELIZATION/metadata.json
+-rw-r--r--   0        0        0     7549 2022-07-11 13:32:13.556194 cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/1l_ANNOTATION_WITH_UPTODATE_MODELIZATION/modelization.json
+-rw-r--r--   0        0        0      498 2022-07-11 12:20:33.448671 cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/1l_ANNOTATION_WITH_UPTODATE_MODELIZATION/sampling.json
+-rw-r--r--   0        0        0     1580 2022-07-11 12:18:44.031863 cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/1l_ANNOTATION_WITH_UPTODATE_MODELIZATION/settings.json
+-rw-r--r--   0        0        0      101 2022-07-11 13:32:13.567680 cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/1l_ANNOTATION_WITH_UPTODATE_MODELIZATION/status.json
+-rw-r--r--   0        0        0     6512 2022-07-11 13:32:09.435685 cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/1l_ANNOTATION_WITH_UPTODATE_MODELIZATION/texts.json
+-rw-r--r--   0        0        0     5469 2022-07-11 13:32:09.842201 cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/1l_ANNOTATION_WITH_UPTODATE_MODELIZATION/vectors.pkl
+-rw-r--r--   0        0        0     2001 2022-07-11 13:32:11.354109 cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/1l_ANNOTATION_WITH_UPTODATE_MODELIZATION/vectors_2D.json
+-rw-r--r--   0        0        0     2773 2022-07-11 13:32:12.581956 cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/1l_ANNOTATION_WITH_UPTODATE_MODELIZATION/vectors_3D.json
+-rw-r--r--   0        0        0      444 2022-07-11 12:14:11.348217 cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/1m_CLUSTERING_TODO/clustering.json
+-rw-r--r--   0        0        0    11444 2022-07-11 13:32:13.084020 cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/1m_CLUSTERING_TODO/constraints.json
+-rw-r--r--   0        0        0     2160 2022-08-23 13:18:42.073502 cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/1m_CLUSTERING_TODO/constraints_manager.pkl
+-rw-r--r--   0        0        0      124 2022-07-11 13:36:31.126577 cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/1m_CLUSTERING_TODO/metadata.json
+-rw-r--r--   0        0        0     7549 2022-07-11 13:32:13.556194 cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/1m_CLUSTERING_TODO/modelization.json
+-rw-r--r--   0        0        0      498 2022-07-11 12:20:33.448671 cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/1m_CLUSTERING_TODO/sampling.json
+-rw-r--r--   0        0        0     1580 2022-07-11 12:18:44.031863 cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/1m_CLUSTERING_TODO/settings.json
+-rw-r--r--   0        0        0       79 2022-07-11 13:35:55.828058 cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/1m_CLUSTERING_TODO/status.json
+-rw-r--r--   0        0        0     6512 2022-07-11 13:32:09.435685 cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/1m_CLUSTERING_TODO/texts.json
+-rw-r--r--   0        0        0     5469 2022-07-11 13:32:09.842201 cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/1m_CLUSTERING_TODO/vectors.pkl
+-rw-r--r--   0        0        0     2001 2022-07-11 13:32:11.354109 cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/1m_CLUSTERING_TODO/vectors_2D.json
+-rw-r--r--   0        0        0     2773 2022-07-11 13:32:12.581956 cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/1m_CLUSTERING_TODO/vectors_3D.json
+-rw-r--r--   0        0        0      444 2022-07-11 12:14:11.348217 cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/1n_CLUSTERING_PENDING/clustering.json
+-rw-r--r--   0        0        0    11444 2022-07-11 13:32:13.084020 cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/1n_CLUSTERING_PENDING/constraints.json
+-rw-r--r--   0        0        0     2160 2022-08-23 13:18:42.080483 cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/1n_CLUSTERING_PENDING/constraints_manager.pkl
+-rw-r--r--   0        0        0      127 2022-07-11 13:38:11.134105 cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/1n_CLUSTERING_PENDING/metadata.json
+-rw-r--r--   0        0        0     7549 2022-07-11 13:32:13.556194 cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/1n_CLUSTERING_PENDING/modelization.json
+-rw-r--r--   0        0        0      498 2022-07-11 12:20:33.448671 cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/1n_CLUSTERING_PENDING/sampling.json
+-rw-r--r--   0        0        0     1580 2022-07-11 12:18:44.031863 cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/1n_CLUSTERING_PENDING/settings.json
+-rw-r--r--   0        0        0      176 2022-08-23 08:03:11.358480 cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/1n_CLUSTERING_PENDING/status.json
+-rw-r--r--   0        0        0     6512 2022-07-11 13:32:09.435685 cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/1n_CLUSTERING_PENDING/texts.json
+-rw-r--r--   0        0        0     5469 2022-07-11 13:32:09.842201 cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/1n_CLUSTERING_PENDING/vectors.pkl
+-rw-r--r--   0        0        0     2001 2022-07-11 13:32:11.354109 cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/1n_CLUSTERING_PENDING/vectors_2D.json
+-rw-r--r--   0        0        0     2773 2022-07-11 13:32:12.581956 cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/1n_CLUSTERING_PENDING/vectors_3D.json
+-rw-r--r--   0        0        0      444 2022-07-11 12:14:11.348217 cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/1o_CLUSTERING_WORKING/clustering.json
+-rw-r--r--   0        0        0    11444 2022-07-11 13:32:13.084020 cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/1o_CLUSTERING_WORKING/constraints.json
+-rw-r--r--   0        0        0     2160 2022-08-23 13:18:42.086467 cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/1o_CLUSTERING_WORKING/constraints_manager.pkl
+-rw-r--r--   0        0        0      127 2022-07-11 13:38:57.822291 cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/1o_CLUSTERING_WORKING/metadata.json
+-rw-r--r--   0        0        0     7549 2022-07-11 13:32:13.556194 cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/1o_CLUSTERING_WORKING/modelization.json
+-rw-r--r--   0        0        0      498 2022-07-11 12:20:33.448671 cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/1o_CLUSTERING_WORKING/sampling.json
+-rw-r--r--   0        0        0     1580 2022-07-11 12:18:44.031863 cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/1o_CLUSTERING_WORKING/settings.json
+-rw-r--r--   0        0        0      163 2022-08-23 08:03:11.356483 cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/1o_CLUSTERING_WORKING/status.json
+-rw-r--r--   0        0        0     6512 2022-07-11 13:32:09.435685 cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/1o_CLUSTERING_WORKING/texts.json
+-rw-r--r--   0        0        0     5469 2022-07-11 13:32:09.842201 cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/1o_CLUSTERING_WORKING/vectors.pkl
+-rw-r--r--   0        0        0     2001 2022-07-11 13:32:11.354109 cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/1o_CLUSTERING_WORKING/vectors_2D.json
+-rw-r--r--   0        0        0     2773 2022-07-11 13:32:12.581956 cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/1o_CLUSTERING_WORKING/vectors_3D.json
+-rw-r--r--   0        0        0      867 2022-07-11 13:37:45.568647 cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/1p_ITERATION_END/clustering.json
+-rw-r--r--   0        0        0    11444 2022-07-11 13:32:13.084020 cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/1p_ITERATION_END/constraints.json
+-rw-r--r--   0        0        0     2160 2022-08-23 13:18:42.092451 cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/1p_ITERATION_END/constraints_manager.pkl
+-rw-r--r--   0        0        0      122 2022-07-11 13:40:36.003123 cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/1p_ITERATION_END/metadata.json
+-rw-r--r--   0        0        0     7549 2022-07-11 13:32:13.556194 cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/1p_ITERATION_END/modelization.json
+-rw-r--r--   0        0        0      498 2022-07-11 12:20:33.448671 cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/1p_ITERATION_END/sampling.json
+-rw-r--r--   0        0        0     1580 2022-07-11 12:18:44.031863 cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/1p_ITERATION_END/settings.json
+-rw-r--r--   0        0        0       77 2022-07-11 13:37:45.590987 cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/1p_ITERATION_END/status.json
+-rw-r--r--   0        0        0     6512 2022-07-11 13:32:09.435685 cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/1p_ITERATION_END/texts.json
+-rw-r--r--   0        0        0     5469 2022-07-11 13:32:09.842201 cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/1p_ITERATION_END/vectors.pkl
+-rw-r--r--   0        0        0     2001 2022-07-11 13:32:11.354109 cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/1p_ITERATION_END/vectors_2D.json
+-rw-r--r--   0        0        0     2773 2022-07-11 13:32:12.581956 cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/1p_ITERATION_END/vectors_3D.json
+-rw-r--r--   0        0        0      867 2022-07-11 13:37:45.568647 cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/2a_SAMPLING_TODO/clustering.json
+-rw-r--r--   0        0        0    11444 2022-07-11 13:32:13.084020 cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/2a_SAMPLING_TODO/constraints.json
+-rw-r--r--   0        0        0     2160 2022-08-23 13:18:42.099434 cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/2a_SAMPLING_TODO/constraints_manager.pkl
+-rw-r--r--   0        0        0      122 2022-07-11 13:40:36.003123 cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/2a_SAMPLING_TODO/metadata.json
+-rw-r--r--   0        0        0     7549 2022-07-11 13:32:13.556194 cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/2a_SAMPLING_TODO/modelization.json
+-rw-r--r--   0        0        0      498 2022-07-11 12:20:33.448671 cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/2a_SAMPLING_TODO/sampling.json
+-rw-r--r--   0        0        0     2627 2022-08-16 13:06:28.980097 cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/2a_SAMPLING_TODO/settings.json
+-rw-r--r--   0        0        0       77 2022-07-26 08:52:16.772181 cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/2a_SAMPLING_TODO/status.json
+-rw-r--r--   0        0        0     6512 2022-07-11 13:32:09.435685 cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/2a_SAMPLING_TODO/texts.json
+-rw-r--r--   0        0        0     5469 2022-07-11 13:32:09.842201 cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/2a_SAMPLING_TODO/vectors.pkl
+-rw-r--r--   0        0        0     2001 2022-07-11 13:32:11.354109 cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/2a_SAMPLING_TODO/vectors_2D.json
+-rw-r--r--   0        0        0     2773 2022-07-11 13:32:12.581956 cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/2a_SAMPLING_TODO/vectors_3D.json
+-rw-r--r--   0        0        0      885 2022-08-16 13:41:53.919265 cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/2b2_SAMPLING_PENDING/clustering.json
+-rw-r--r--   0        0        0     9980 2022-07-11 12:20:33.453660 cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/2b2_SAMPLING_PENDING/constraints.json
+-rw-r--r--   0        0        0     1880 2022-08-23 13:18:42.105416 cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/2b2_SAMPLING_PENDING/constraints_manager.pkl
+-rw-r--r--   0        0        0      122 2022-07-11 13:40:36.003123 cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/2b2_SAMPLING_PENDING/metadata.json
+-rw-r--r--   0        0        0     7549 2022-07-11 13:32:13.556194 cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/2b2_SAMPLING_PENDING/modelization.json
+-rw-r--r--   0        0        0      498 2022-08-18 10:46:51.121529 cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/2b2_SAMPLING_PENDING/sampling.json
+-rw-r--r--   0        0        0     2627 2022-08-16 13:06:04.636697 cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/2b2_SAMPLING_PENDING/settings.json
+-rw-r--r--   0        0        0      175 2022-08-23 08:03:11.350499 cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/2b2_SAMPLING_PENDING/status.json
+-rw-r--r--   0        0        0     6513 2022-08-16 13:42:08.834581 cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/2b2_SAMPLING_PENDING/texts.json
+-rw-r--r--   0        0        0     5825 2022-07-11 12:10:24.327037 cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/2b2_SAMPLING_PENDING/vectors.pkl
+-rw-r--r--   0        0        0     2106 2022-07-11 12:10:25.284783 cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/2b2_SAMPLING_PENDING/vectors_2D.json
+-rw-r--r--   0        0        0     2904 2022-07-11 12:10:26.615845 cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/2b2_SAMPLING_PENDING/vectors_3D.json
+-rw-r--r--   0        0        0      867 2022-07-11 13:37:45.568647 cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/2b_SAMPLING_PENDING/clustering.json
+-rw-r--r--   0        0        0    11444 2022-07-11 13:32:13.084020 cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/2b_SAMPLING_PENDING/constraints.json
+-rw-r--r--   0        0        0     2160 2022-08-23 13:18:42.111400 cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/2b_SAMPLING_PENDING/constraints_manager.pkl
+-rw-r--r--   0        0        0      122 2022-07-11 13:40:36.003123 cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/2b_SAMPLING_PENDING/metadata.json
+-rw-r--r--   0        0        0     7549 2022-07-11 13:32:13.556194 cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/2b_SAMPLING_PENDING/modelization.json
+-rw-r--r--   0        0        0      498 2022-07-11 12:20:33.448671 cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/2b_SAMPLING_PENDING/sampling.json
+-rw-r--r--   0        0        0     2627 2022-08-16 13:06:04.636697 cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/2b_SAMPLING_PENDING/settings.json
+-rw-r--r--   0        0        0      175 2022-08-23 08:03:11.351497 cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/2b_SAMPLING_PENDING/status.json
+-rw-r--r--   0        0        0     6512 2022-07-11 13:32:09.435685 cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/2b_SAMPLING_PENDING/texts.json
+-rw-r--r--   0        0        0     5469 2022-07-11 13:32:09.842201 cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/2b_SAMPLING_PENDING/vectors.pkl
+-rw-r--r--   0        0        0     2001 2022-07-11 13:32:11.354109 cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/2b_SAMPLING_PENDING/vectors_2D.json
+-rw-r--r--   0        0        0     2773 2022-07-11 13:32:12.581956 cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/2b_SAMPLING_PENDING/vectors_3D.json
+-rw-r--r--   0        0        0      867 2022-07-11 13:37:45.568647 cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/2d_ANNOTATION_WITH_UPTODATE_MODELIZATION/clustering.json
+-rw-r--r--   0        0        0    64545 2022-08-16 13:19:03.162721 cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/2d_ANNOTATION_WITH_UPTODATE_MODELIZATION/constraints.json
+-rw-r--r--   0        0        0     2160 2022-08-23 13:18:42.118384 cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/2d_ANNOTATION_WITH_UPTODATE_MODELIZATION/constraints_manager.pkl
+-rw-r--r--   0        0        0      146 2022-07-11 13:45:33.025114 cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/2d_ANNOTATION_WITH_UPTODATE_MODELIZATION/metadata.json
+-rw-r--r--   0        0        0     7549 2022-07-11 13:32:13.556194 cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/2d_ANNOTATION_WITH_UPTODATE_MODELIZATION/modelization.json
+-rw-r--r--   0        0        0     5807 2022-08-18 10:46:39.012624 cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/2d_ANNOTATION_WITH_UPTODATE_MODELIZATION/sampling.json
+-rw-r--r--   0        0        0     2627 2022-08-16 13:06:18.718616 cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/2d_ANNOTATION_WITH_UPTODATE_MODELIZATION/settings.json
+-rw-r--r--   0        0        0      101 2022-07-11 13:45:09.965237 cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/2d_ANNOTATION_WITH_UPTODATE_MODELIZATION/status.json
+-rw-r--r--   0        0        0     6512 2022-07-11 13:32:09.435685 cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/2d_ANNOTATION_WITH_UPTODATE_MODELIZATION/texts.json
+-rw-r--r--   0        0        0     5469 2022-07-11 13:32:09.842201 cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/2d_ANNOTATION_WITH_UPTODATE_MODELIZATION/vectors.pkl
+-rw-r--r--   0        0        0     2001 2022-07-11 13:32:11.354109 cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/2d_ANNOTATION_WITH_UPTODATE_MODELIZATION/vectors_2D.json
+-rw-r--r--   0        0        0     2773 2022-07-11 13:32:12.581956 cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/2d_ANNOTATION_WITH_UPTODATE_MODELIZATION/vectors_3D.json
+-rw-r--r--   0        0        0     2443 2022-07-19 13:23:52.519541 cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/archive-0a_INITIALIZATION_WITHOUT_MODELIZATION.zip
+-rw-r--r--   0        0        0     4445 2022-07-11 14:10:29.043689 cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/archive-1b_SAMPLING_PENDING.zip
+-rw-r--r--   0        0        0     4930 2022-07-11 14:00:42.949467 cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/archive-1d_ANNOTATION_WITH_UPTODATE_MODELIZATION.zip
+-rw-r--r--   0        0        0     5368 2022-07-21 13:33:48.984320 cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/archive-1h_ANNOTATION_WITH_OUTDATED_MODELIZATION_WITH_CONFLICTS.zip
+-rw-r--r--   0        0        0     5422 2022-07-11 14:11:07.712387 cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/archive-1j_ANNOTATION_WITH_PENDING_MODELIZATION_WITH_CONFLICTS.zip
+-rw-r--r--   0        0        0     5367 2022-07-20 08:54:04.397687 cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/archive-1l_ANNOTATION_WITH_UPTODATE_MODELIZATION.zip
+-rw-r--r--   0        0        0    11846 2022-07-19 13:18:15.405915 cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/archive-1o_CLUSTERING_WORKING.zip
+-rw-r--r--   0        0        0     8324 2022-07-19 13:18:57.703046 cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/archive-1p_ITERATION_END.zip
+-rw-r--r--   0        0        0     3361 2022-07-19 13:52:29.115912 cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/archive-ERROR_bad_archive.zip
+-rw-r--r--   0        0        0     4439 2022-07-19 13:18:34.810168 cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/archive-ERROR_metadata_bad_creation_timestamp.zip
+-rw-r--r--   0        0        0     4450 2022-07-19 13:18:53.508055 cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/archive-ERROR_metadata_bad_project_name.zip
+-rw-r--r--   0        0        0     4415 2022-07-19 13:19:23.354348 cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/archive-ERROR_metadata_missing_creation_timestamp.zip
+-rw-r--r--   0        0        0     4424 2022-07-19 13:19:38.863582 cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/archive-ERROR_metadata_missing_project_name.zip
+-rw-r--r--   0        0        0     1185 2022-07-19 13:31:51.308161 cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/archive-ERROR_missing_files.zip
+-rw-r--r--   0        0        0     4428 2022-07-19 13:20:13.283333 cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/archive-ERROR_status_bad_state.zip
+-rw-r--r--   0        0        0     4409 2022-07-19 13:20:35.454944 cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/archive-ERROR_status_missing_state.zip
+-rw-r--r--   0        0        0     1098 2022-07-12 15:28:00.547593 cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/dummy_24.csv
+-rw-r--r--   0        0        0     1075 2022-07-12 14:12:39.131119 cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/dummy_24.txt
+-rw-r--r--   0        0        0     9095 2022-07-11 11:58:18.587515 cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/dummy_24.xlsx
+-rw-r--r--   0        0        0     1110 2022-07-11 11:57:06.067159 cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/dummy_24_err.csv
+-rw-r--r--   0        0        0     9122 2022-07-11 11:58:06.501182 cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/dummy_24_err.xlsx
+-rw-r--r--   0        0        0        2 2022-07-11 12:07:21.312463 cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/import_0y0_INITIALIZATION_WITHOUT_MODELIZATION/clustering.json
+-rw-r--r--   0        0        0        2 2022-07-11 12:07:21.271572 cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/import_0y0_INITIALIZATION_WITHOUT_MODELIZATION/constraints.json
+-rw-r--r--   0        0        0      152 2022-07-29 10:04:12.529088 cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/import_0y0_INITIALIZATION_WITHOUT_MODELIZATION/metadata.json
+-rw-r--r--   0        0        0     3045 2022-07-11 12:07:21.303486 cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/import_0y0_INITIALIZATION_WITHOUT_MODELIZATION/modelization.json
+-rw-r--r--   0        0        0        2 2022-07-11 12:07:21.309471 cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/import_0y0_INITIALIZATION_WITHOUT_MODELIZATION/sampling.json
+-rw-r--r--   0        0        0      696 2022-07-11 12:13:45.311609 cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/import_0y0_INITIALIZATION_WITHOUT_MODELIZATION/settings.json
+-rw-r--r--   0        0        0       99 2022-07-11 12:07:21.264592 cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/import_0y0_INITIALIZATION_WITHOUT_MODELIZATION/status.json
+-rw-r--r--   0        0        0     6659 2022-07-11 12:07:21.267583 cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/import_0y0_INITIALIZATION_WITHOUT_MODELIZATION/texts.json
+-rw-r--r--   0        0        0        2 2022-07-11 12:07:21.312463 cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/import_0y1_INITIALIZATION_WITH_PENDING_MODELIZATION/clustering.json
+-rw-r--r--   0        0        0        2 2022-07-11 12:07:21.271572 cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/import_0y1_INITIALIZATION_WITH_PENDING_MODELIZATION/constraints.json
+-rw-r--r--   0        0        0      157 2022-07-29 10:04:49.540024 cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/import_0y1_INITIALIZATION_WITH_PENDING_MODELIZATION/metadata.json
+-rw-r--r--   0        0        0     3045 2022-07-11 12:07:21.303486 cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/import_0y1_INITIALIZATION_WITH_PENDING_MODELIZATION/modelization.json
+-rw-r--r--   0        0        0        2 2022-07-11 12:07:21.309471 cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/import_0y1_INITIALIZATION_WITH_PENDING_MODELIZATION/sampling.json
+-rw-r--r--   0        0        0      696 2022-07-11 12:13:45.311609 cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/import_0y1_INITIALIZATION_WITH_PENDING_MODELIZATION/settings.json
+-rw-r--r--   0        0        0      198 2022-08-23 08:03:11.350499 cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/import_0y1_INITIALIZATION_WITH_PENDING_MODELIZATION/status.json
+-rw-r--r--   0        0        0     6659 2022-07-11 12:07:21.267583 cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/import_0y1_INITIALIZATION_WITH_PENDING_MODELIZATION/texts.json
+-rw-r--r--   0        0        0        2 2022-07-11 12:07:21.312463 cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/import_0y2_INITIALIZATION_WITH_WORKING_MODELIZATION/clustering.json
+-rw-r--r--   0        0        0        2 2022-07-11 12:07:21.271572 cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/import_0y2_INITIALIZATION_WITH_WORKING_MODELIZATION/constraints.json
+-rw-r--r--   0        0        0      157 2022-07-29 10:05:16.190204 cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/import_0y2_INITIALIZATION_WITH_WORKING_MODELIZATION/metadata.json
+-rw-r--r--   0        0        0     3045 2022-07-11 12:07:21.303486 cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/import_0y2_INITIALIZATION_WITH_WORKING_MODELIZATION/modelization.json
+-rw-r--r--   0        0        0        2 2022-07-11 12:07:21.309471 cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/import_0y2_INITIALIZATION_WITH_WORKING_MODELIZATION/sampling.json
+-rw-r--r--   0        0        0      696 2022-07-11 12:13:45.311609 cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/import_0y2_INITIALIZATION_WITH_WORKING_MODELIZATION/settings.json
+-rw-r--r--   0        0        0      175 2022-08-23 08:03:11.350499 cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/import_0y2_INITIALIZATION_WITH_WORKING_MODELIZATION/status.json
+-rw-r--r--   0        0        0     6659 2022-07-11 12:07:21.267583 cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/import_0y2_INITIALIZATION_WITH_WORKING_MODELIZATION/texts.json
+-rw-r--r--   0        0        0      444 2022-07-29 09:18:22.863211 cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/import_1w0_IMPORT_AT_SAMPLING_STEP_WITHOUT_MODELIZATION/clustering.json
+-rw-r--r--   0        0        0        2 2022-07-29 09:18:22.855235 cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/import_1w0_IMPORT_AT_SAMPLING_STEP_WITHOUT_MODELIZATION/constraints.json
+-rw-r--r--   0        0        0      161 2022-07-29 10:14:43.461129 cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/import_1w0_IMPORT_AT_SAMPLING_STEP_WITHOUT_MODELIZATION/metadata.json
+-rw-r--r--   0        0        0     3045 2022-07-29 09:18:22.868198 cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/import_1w0_IMPORT_AT_SAMPLING_STEP_WITHOUT_MODELIZATION/modelization.json
+-rw-r--r--   0        0        0        2 2022-07-29 09:18:22.861216 cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/import_1w0_IMPORT_AT_SAMPLING_STEP_WITHOUT_MODELIZATION/sampling.json
+-rw-r--r--   0        0        0     1580 2022-07-29 09:18:22.858225 cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/import_1w0_IMPORT_AT_SAMPLING_STEP_WITHOUT_MODELIZATION/settings.json
+-rw-r--r--   0        0        0      108 2022-07-29 10:14:52.344716 cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/import_1w0_IMPORT_AT_SAMPLING_STEP_WITHOUT_MODELIZATION/status.json
+-rw-r--r--   0        0        0     6513 2022-07-11 12:10:23.869094 cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/import_1w0_IMPORT_AT_SAMPLING_STEP_WITHOUT_MODELIZATION/texts.json
+-rw-r--r--   0        0        0      444 2022-07-29 09:18:22.863211 cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/import_1w1_IMPORT_AT_SAMPLING_STEP_WITH_PENDING_MODELIZATION/clustering.json
+-rw-r--r--   0        0        0        2 2022-07-29 09:18:22.855235 cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/import_1w1_IMPORT_AT_SAMPLING_STEP_WITH_PENDING_MODELIZATION/constraints.json
+-rw-r--r--   0        0        0      166 2022-07-29 10:28:15.424848 cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/import_1w1_IMPORT_AT_SAMPLING_STEP_WITH_PENDING_MODELIZATION/metadata.json
+-rw-r--r--   0        0        0     3045 2022-07-29 09:18:22.868198 cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/import_1w1_IMPORT_AT_SAMPLING_STEP_WITH_PENDING_MODELIZATION/modelization.json
+-rw-r--r--   0        0        0        2 2022-07-29 09:18:22.861216 cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/import_1w1_IMPORT_AT_SAMPLING_STEP_WITH_PENDING_MODELIZATION/sampling.json
+-rw-r--r--   0        0        0     1580 2022-07-29 09:18:22.858225 cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/import_1w1_IMPORT_AT_SAMPLING_STEP_WITH_PENDING_MODELIZATION/settings.json
+-rw-r--r--   0        0        0      207 2022-08-23 08:03:11.350499 cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/import_1w1_IMPORT_AT_SAMPLING_STEP_WITH_PENDING_MODELIZATION/status.json
+-rw-r--r--   0        0        0     6513 2022-07-11 12:10:23.869094 cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/import_1w1_IMPORT_AT_SAMPLING_STEP_WITH_PENDING_MODELIZATION/texts.json
+-rw-r--r--   0        0        0      444 2022-07-29 09:18:22.863211 cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/import_1w2_IMPORT_AT_SAMPLING_STEP_WORKING_MODELIZATION/clustering.json
+-rw-r--r--   0        0        0        2 2022-07-29 09:18:22.855235 cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/import_1w2_IMPORT_AT_SAMPLING_STEP_WORKING_MODELIZATION/constraints.json
+-rw-r--r--   0        0        0      161 2022-07-29 10:26:02.398488 cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/import_1w2_IMPORT_AT_SAMPLING_STEP_WORKING_MODELIZATION/metadata.json
+-rw-r--r--   0        0        0     3045 2022-07-29 09:18:22.868198 cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/import_1w2_IMPORT_AT_SAMPLING_STEP_WORKING_MODELIZATION/modelization.json
+-rw-r--r--   0        0        0        2 2022-07-29 09:18:22.861216 cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/import_1w2_IMPORT_AT_SAMPLING_STEP_WORKING_MODELIZATION/sampling.json
+-rw-r--r--   0        0        0     1580 2022-07-29 09:18:22.858225 cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/import_1w2_IMPORT_AT_SAMPLING_STEP_WORKING_MODELIZATION/settings.json
+-rw-r--r--   0        0        0      184 2022-08-23 08:03:11.350499 cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/import_1w2_IMPORT_AT_SAMPLING_STEP_WORKING_MODELIZATION/status.json
+-rw-r--r--   0        0        0     6513 2022-07-11 12:10:23.869094 cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/import_1w2_IMPORT_AT_SAMPLING_STEP_WORKING_MODELIZATION/texts.json
+-rw-r--r--   0        0        0      444 2022-07-29 09:19:07.962559 cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/import_1x0_IMPORT_AT_ANNOTATION_STEP_WITHOUT_MODELIZATION/clustering.json
+-rw-r--r--   0        0        0    11444 2022-07-11 13:32:13.084020 cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/import_1x0_IMPORT_AT_ANNOTATION_STEP_WITHOUT_MODELIZATION/constraints.json
+-rw-r--r--   0        0        0      163 2022-07-29 10:16:34.037911 cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/import_1x0_IMPORT_AT_ANNOTATION_STEP_WITHOUT_MODELIZATION/metadata.json
+-rw-r--r--   0        0        0     7676 2022-08-16 09:24:59.463501 cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/import_1x0_IMPORT_AT_ANNOTATION_STEP_WITHOUT_MODELIZATION/modelization.json
+-rw-r--r--   0        0        0      498 2022-07-29 09:19:07.959568 cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/import_1x0_IMPORT_AT_ANNOTATION_STEP_WITHOUT_MODELIZATION/sampling.json
+-rw-r--r--   0        0        0     1580 2022-07-29 09:19:07.956576 cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/import_1x0_IMPORT_AT_ANNOTATION_STEP_WITHOUT_MODELIZATION/settings.json
+-rw-r--r--   0        0        0      110 2022-07-29 09:19:07.946602 cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/import_1x0_IMPORT_AT_ANNOTATION_STEP_WITHOUT_MODELIZATION/status.json
+-rw-r--r--   0        0        0     6513 2022-07-11 12:10:23.869094 cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/import_1x0_IMPORT_AT_ANNOTATION_STEP_WITHOUT_MODELIZATION/texts.json
+-rw-r--r--   0        0        0      444 2022-07-29 09:19:07.962559 cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/import_1x1_IMPORT_AT_ANNOTATION_STEP_WITH_PENDING_MODELIZATION/clustering.json
+-rw-r--r--   0        0        0    11446 2022-08-16 08:43:22.934424 cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/import_1x1_IMPORT_AT_ANNOTATION_STEP_WITH_PENDING_MODELIZATION/constraints.json
+-rw-r--r--   0        0        0      168 2022-07-29 10:28:42.145270 cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/import_1x1_IMPORT_AT_ANNOTATION_STEP_WITH_PENDING_MODELIZATION/metadata.json
+-rw-r--r--   0        0        0     7676 2022-08-16 09:24:50.960133 cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/import_1x1_IMPORT_AT_ANNOTATION_STEP_WITH_PENDING_MODELIZATION/modelization.json
+-rw-r--r--   0        0        0      498 2022-07-29 09:19:07.959568 cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/import_1x1_IMPORT_AT_ANNOTATION_STEP_WITH_PENDING_MODELIZATION/sampling.json
+-rw-r--r--   0        0        0     1580 2022-07-29 09:19:07.956576 cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/import_1x1_IMPORT_AT_ANNOTATION_STEP_WITH_PENDING_MODELIZATION/settings.json
+-rw-r--r--   0        0        0      209 2022-08-23 08:03:11.345513 cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/import_1x1_IMPORT_AT_ANNOTATION_STEP_WITH_PENDING_MODELIZATION/status.json
+-rw-r--r--   0        0        0     6513 2022-07-11 12:10:23.869094 cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/import_1x1_IMPORT_AT_ANNOTATION_STEP_WITH_PENDING_MODELIZATION/texts.json
+-rw-r--r--   0        0        0      444 2022-07-29 09:19:07.962559 cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/import_1x2_IMPORT_AT_ANNOTATION_STEP_WORKING_MODELIZATION/clustering.json
+-rw-r--r--   0        0        0    11444 2022-07-11 13:32:13.084020 cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/import_1x2_IMPORT_AT_ANNOTATION_STEP_WORKING_MODELIZATION/constraints.json
+-rw-r--r--   0        0        0      163 2022-07-29 10:26:35.966938 cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/import_1x2_IMPORT_AT_ANNOTATION_STEP_WORKING_MODELIZATION/metadata.json
+-rw-r--r--   0        0        0     7676 2022-08-16 09:25:56.717172 cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/import_1x2_IMPORT_AT_ANNOTATION_STEP_WORKING_MODELIZATION/modelization.json
+-rw-r--r--   0        0        0      498 2022-07-29 09:19:07.959568 cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/import_1x2_IMPORT_AT_ANNOTATION_STEP_WORKING_MODELIZATION/sampling.json
+-rw-r--r--   0        0        0     1580 2022-07-29 09:19:07.956576 cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/import_1x2_IMPORT_AT_ANNOTATION_STEP_WORKING_MODELIZATION/settings.json
+-rw-r--r--   0        0        0      186 2022-08-23 08:03:11.344515 cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/import_1x2_IMPORT_AT_ANNOTATION_STEP_WORKING_MODELIZATION/status.json
+-rw-r--r--   0        0        0     6513 2022-07-11 12:10:23.869094 cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/import_1x2_IMPORT_AT_ANNOTATION_STEP_WORKING_MODELIZATION/texts.json
+-rw-r--r--   0        0        0      444 2022-07-29 09:19:30.708376 cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/import_1y0_IMPORT_AT_CLUSTERING_STEP_WITHOUT_MODELIZATION/clustering.json
+-rw-r--r--   0        0        0    11444 2022-07-29 09:19:30.702390 cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/import_1y0_IMPORT_AT_CLUSTERING_STEP_WITHOUT_MODELIZATION/constraints.json
+-rw-r--r--   0        0        0      163 2022-07-29 10:16:45.014900 cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/import_1y0_IMPORT_AT_CLUSTERING_STEP_WITHOUT_MODELIZATION/metadata.json
+-rw-r--r--   0        0        0     7676 2022-08-16 09:26:03.311603 cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/import_1y0_IMPORT_AT_CLUSTERING_STEP_WITHOUT_MODELIZATION/modelization.json
+-rw-r--r--   0        0        0      498 2022-07-29 09:19:30.706380 cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/import_1y0_IMPORT_AT_CLUSTERING_STEP_WITHOUT_MODELIZATION/sampling.json
+-rw-r--r--   0        0        0     1580 2022-07-29 09:19:30.704382 cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/import_1y0_IMPORT_AT_CLUSTERING_STEP_WITHOUT_MODELIZATION/settings.json
+-rw-r--r--   0        0        0      110 2022-07-29 09:19:30.662979 cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/import_1y0_IMPORT_AT_CLUSTERING_STEP_WITHOUT_MODELIZATION/status.json
+-rw-r--r--   0        0        0     6513 2022-07-11 12:10:23.869094 cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/import_1y0_IMPORT_AT_CLUSTERING_STEP_WITHOUT_MODELIZATION/texts.json
+-rw-r--r--   0        0        0      444 2022-07-29 09:19:30.708376 cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/import_1y1_IMPORT_AT_CLUSTERING_STEP_WITH_PENDING_MODELIZATION/clustering.json
+-rw-r--r--   0        0        0    11444 2022-07-29 09:19:30.702390 cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/import_1y1_IMPORT_AT_CLUSTERING_STEP_WITH_PENDING_MODELIZATION/constraints.json
+-rw-r--r--   0        0        0      168 2022-07-29 10:28:57.082029 cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/import_1y1_IMPORT_AT_CLUSTERING_STEP_WITH_PENDING_MODELIZATION/metadata.json
+-rw-r--r--   0        0        0     7676 2022-08-16 09:26:10.886957 cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/import_1y1_IMPORT_AT_CLUSTERING_STEP_WITH_PENDING_MODELIZATION/modelization.json
+-rw-r--r--   0        0        0      498 2022-07-29 09:19:30.706380 cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/import_1y1_IMPORT_AT_CLUSTERING_STEP_WITH_PENDING_MODELIZATION/sampling.json
+-rw-r--r--   0        0        0     1580 2022-07-29 09:19:30.704382 cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/import_1y1_IMPORT_AT_CLUSTERING_STEP_WITH_PENDING_MODELIZATION/settings.json
+-rw-r--r--   0        0        0      209 2022-08-23 08:03:11.342520 cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/import_1y1_IMPORT_AT_CLUSTERING_STEP_WITH_PENDING_MODELIZATION/status.json
+-rw-r--r--   0        0        0     6513 2022-07-11 12:10:23.869094 cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/import_1y1_IMPORT_AT_CLUSTERING_STEP_WITH_PENDING_MODELIZATION/texts.json
+-rw-r--r--   0        0        0      444 2022-07-29 09:19:30.708376 cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/import_1y2_IMPORT_AT_CLUSTERING_STEP_WORKING_MODELIZATION/clustering.json
+-rw-r--r--   0        0        0    11444 2022-07-29 09:19:30.702390 cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/import_1y2_IMPORT_AT_CLUSTERING_STEP_WORKING_MODELIZATION/constraints.json
+-rw-r--r--   0        0        0      163 2022-07-29 10:26:51.304470 cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/import_1y2_IMPORT_AT_CLUSTERING_STEP_WORKING_MODELIZATION/metadata.json
+-rw-r--r--   0        0        0     7676 2022-08-16 09:26:18.210742 cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/import_1y2_IMPORT_AT_CLUSTERING_STEP_WORKING_MODELIZATION/modelization.json
+-rw-r--r--   0        0        0      498 2022-07-29 09:19:30.706380 cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/import_1y2_IMPORT_AT_CLUSTERING_STEP_WORKING_MODELIZATION/sampling.json
+-rw-r--r--   0        0        0     1580 2022-07-29 09:19:30.704382 cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/import_1y2_IMPORT_AT_CLUSTERING_STEP_WORKING_MODELIZATION/settings.json
+-rw-r--r--   0        0        0      186 2022-08-23 08:03:11.338532 cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/import_1y2_IMPORT_AT_CLUSTERING_STEP_WORKING_MODELIZATION/status.json
+-rw-r--r--   0        0        0     6513 2022-07-11 12:10:23.869094 cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/import_1y2_IMPORT_AT_CLUSTERING_STEP_WORKING_MODELIZATION/texts.json
+-rw-r--r--   0        0        0      867 2022-07-29 09:19:45.960931 cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/import_1z0_IMPORT_AT_ITERATION_END_WITHOUT_MODELIZATION/clustering.json
+-rw-r--r--   0        0        0    11444 2022-07-29 09:19:45.951958 cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/import_1z0_IMPORT_AT_ITERATION_END_WITHOUT_MODELIZATION/constraints.json
+-rw-r--r--   0        0        0      161 2022-07-29 10:17:15.766568 cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/import_1z0_IMPORT_AT_ITERATION_END_WITHOUT_MODELIZATION/metadata.json
+-rw-r--r--   0        0        0     7676 2022-08-16 09:26:25.021358 cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/import_1z0_IMPORT_AT_ITERATION_END_WITHOUT_MODELIZATION/modelization.json
+-rw-r--r--   0        0        0      498 2022-07-29 09:19:45.957939 cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/import_1z0_IMPORT_AT_ITERATION_END_WITHOUT_MODELIZATION/sampling.json
+-rw-r--r--   0        0        0     1580 2022-07-29 09:19:45.954954 cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/import_1z0_IMPORT_AT_ITERATION_END_WITHOUT_MODELIZATION/settings.json
+-rw-r--r--   0        0        0      108 2022-07-29 09:19:45.942978 cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/import_1z0_IMPORT_AT_ITERATION_END_WITHOUT_MODELIZATION/status.json
+-rw-r--r--   0        0        0     6513 2022-07-11 12:10:23.869094 cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/import_1z0_IMPORT_AT_ITERATION_END_WITHOUT_MODELIZATION/texts.json
+-rw-r--r--   0        0        0      867 2022-08-16 08:30:23.075267 cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/import_1z1_IMPORT_AT_ITERATION_END_WITH_PENDING_MODELIZATION/clustering.json
+-rw-r--r--   0        0        0    11444 2022-07-29 09:19:45.951958 cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/import_1z1_IMPORT_AT_ITERATION_END_WITH_PENDING_MODELIZATION/constraints.json
+-rw-r--r--   0        0        0      166 2022-07-29 10:29:09.786464 cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/import_1z1_IMPORT_AT_ITERATION_END_WITH_PENDING_MODELIZATION/metadata.json
+-rw-r--r--   0        0        0     7676 2022-08-16 09:26:32.211112 cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/import_1z1_IMPORT_AT_ITERATION_END_WITH_PENDING_MODELIZATION/modelization.json
+-rw-r--r--   0        0        0      498 2022-07-29 09:19:45.957939 cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/import_1z1_IMPORT_AT_ITERATION_END_WITH_PENDING_MODELIZATION/sampling.json
+-rw-r--r--   0        0        0     1580 2022-07-29 09:19:45.954954 cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/import_1z1_IMPORT_AT_ITERATION_END_WITH_PENDING_MODELIZATION/settings.json
+-rw-r--r--   0        0        0      207 2022-08-23 08:03:11.338532 cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/import_1z1_IMPORT_AT_ITERATION_END_WITH_PENDING_MODELIZATION/status.json
+-rw-r--r--   0        0        0     6513 2022-07-11 12:10:23.869094 cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/import_1z1_IMPORT_AT_ITERATION_END_WITH_PENDING_MODELIZATION/texts.json
+-rw-r--r--   0        0        0      867 2022-07-29 09:19:45.960931 cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/import_1z2_IMPORT_AT_ITERATION_END_WORKING_MODELIZATION/clustering.json
+-rw-r--r--   0        0        0    11444 2022-07-29 09:19:45.951958 cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/import_1z2_IMPORT_AT_ITERATION_END_WORKING_MODELIZATION/constraints.json
+-rw-r--r--   0        0        0      161 2022-07-29 10:27:07.008169 cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/import_1z2_IMPORT_AT_ITERATION_END_WORKING_MODELIZATION/metadata.json
+-rw-r--r--   0        0        0     7676 2022-08-16 09:26:39.280399 cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/import_1z2_IMPORT_AT_ITERATION_END_WORKING_MODELIZATION/modelization.json
+-rw-r--r--   0        0        0      498 2022-07-29 09:19:45.957939 cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/import_1z2_IMPORT_AT_ITERATION_END_WORKING_MODELIZATION/sampling.json
+-rw-r--r--   0        0        0     1580 2022-07-29 09:19:45.954954 cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/import_1z2_IMPORT_AT_ITERATION_END_WORKING_MODELIZATION/settings.json
+-rw-r--r--   0        0        0      184 2022-08-23 08:03:11.338532 cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/import_1z2_IMPORT_AT_ITERATION_END_WORKING_MODELIZATION/status.json
+-rw-r--r--   0        0        0     6513 2022-07-11 12:10:23.869094 cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/import_1z2_IMPORT_AT_ITERATION_END_WORKING_MODELIZATION/texts.json
+-rw-r--r--   0        0        0        2 2022-07-11 12:07:21.312463 cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/import_error_0y1_INITIALIZATION_WITH_PENDING_MODELIZATION/clustering.json
+-rw-r--r--   0        0        0     1810 2022-07-29 10:12:35.231746 cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/import_error_0y1_INITIALIZATION_WITH_PENDING_MODELIZATION/constraints.json
+-rw-r--r--   0        0        0      163 2022-07-29 10:07:25.679543 cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/import_error_0y1_INITIALIZATION_WITH_PENDING_MODELIZATION/metadata.json
+-rw-r--r--   0        0        0     3045 2022-07-11 12:07:21.303486 cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/import_error_0y1_INITIALIZATION_WITH_PENDING_MODELIZATION/modelization.json
+-rw-r--r--   0        0        0        2 2022-07-11 12:07:21.309471 cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/import_error_0y1_INITIALIZATION_WITH_PENDING_MODELIZATION/sampling.json
+-rw-r--r--   0        0        0      696 2022-07-11 12:13:45.311609 cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/import_error_0y1_INITIALIZATION_WITH_PENDING_MODELIZATION/settings.json
+-rw-r--r--   0        0        0      198 2022-08-23 08:03:11.333544 cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/import_error_0y1_INITIALIZATION_WITH_PENDING_MODELIZATION/status.json
+-rw-r--r--   0        0        0     6659 2022-08-16 08:35:06.321495 cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/import_error_0y1_INITIALIZATION_WITH_PENDING_MODELIZATION/texts.json
+-rw-r--r--   0        0        0        2 2022-07-11 12:07:21.312463 cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/import_error_0y3_INITIALIZATION_WITH_ERRORS/clustering.json
+-rw-r--r--   0        0        0     1809 2022-07-29 11:06:31.807149 cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/import_error_0y3_INITIALIZATION_WITH_ERRORS/constraints.json
+-rw-r--r--   0        0        0     1952 2022-08-23 13:18:42.129355 cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/import_error_0y3_INITIALIZATION_WITH_ERRORS/constraints_manager.pkl
+-rw-r--r--   0        0        0      149 2022-07-29 11:03:08.541867 cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/import_error_0y3_INITIALIZATION_WITH_ERRORS/metadata.json
+-rw-r--r--   0        0        0     3295 2022-07-29 11:06:32.237676 cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/import_error_0y3_INITIALIZATION_WITH_ERRORS/modelization.json
+-rw-r--r--   0        0        0        2 2022-07-11 12:07:21.309471 cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/import_error_0y3_INITIALIZATION_WITH_ERRORS/sampling.json
+-rw-r--r--   0        0        0      696 2022-07-11 12:13:45.311609 cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/import_error_0y3_INITIALIZATION_WITH_ERRORS/settings.json
+-rw-r--r--   0        0        0       90 2022-07-29 11:06:32.250642 cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/import_error_0y3_INITIALIZATION_WITH_ERRORS/status.json
+-rw-r--r--   0        0        0     6659 2022-08-16 08:35:15.548914 cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/import_error_0y3_INITIALIZATION_WITH_ERRORS/texts.json
+-rw-r--r--   0        0        0     5825 2022-07-29 11:06:29.081110 cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/import_error_0y3_INITIALIZATION_WITH_ERRORS/vectors.pkl
+-rw-r--r--   0        0        0     2106 2022-07-29 11:06:30.058680 cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/import_error_0y3_INITIALIZATION_WITH_ERRORS/vectors_2D.json
+-rw-r--r--   0        0        0     2904 2022-07-29 11:06:31.334405 cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/import_error_0y3_INITIALIZATION_WITH_ERRORS/vectors_3D.json
+-rw-r--r--   0        0        0      444 2022-08-16 08:29:07.499761 cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/import_error_1w1_IMPORT_AT_SAMPLING_STEP_WITH_PENDING_MODELIZATION/clustering.json
+-rw-r--r--   0        0        0     1810 2022-07-29 10:12:35.231746 cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/import_error_1w1_IMPORT_AT_SAMPLING_STEP_WITH_PENDING_MODELIZATION/constraints.json
+-rw-r--r--   0        0        0      163 2022-07-29 10:07:25.679543 cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/import_error_1w1_IMPORT_AT_SAMPLING_STEP_WITH_PENDING_MODELIZATION/metadata.json
+-rw-r--r--   0        0        0     3045 2022-07-11 12:07:21.303486 cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/import_error_1w1_IMPORT_AT_SAMPLING_STEP_WITH_PENDING_MODELIZATION/modelization.json
+-rw-r--r--   0        0        0        2 2022-07-11 12:07:21.309471 cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/import_error_1w1_IMPORT_AT_SAMPLING_STEP_WITH_PENDING_MODELIZATION/sampling.json
+-rw-r--r--   0        0        0     1580 2022-08-16 08:27:13.966013 cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/import_error_1w1_IMPORT_AT_SAMPLING_STEP_WITH_PENDING_MODELIZATION/settings.json
+-rw-r--r--   0        0        0      207 2022-08-23 08:03:11.333544 cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/import_error_1w1_IMPORT_AT_SAMPLING_STEP_WITH_PENDING_MODELIZATION/status.json
+-rw-r--r--   0        0        0     6513 2022-07-11 12:10:23.869094 cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/import_error_1w1_IMPORT_AT_SAMPLING_STEP_WITH_PENDING_MODELIZATION/texts.json
+-rw-r--r--   0        0        0      444 2022-08-16 08:29:14.945429 cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/import_error_1w3_IMPORT_AT_SAMPLING_STEP_WITH_ERRORS/clustering.json
+-rw-r--r--   0        0        0     1809 2022-07-29 11:07:16.025511 cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/import_error_1w3_IMPORT_AT_SAMPLING_STEP_WITH_ERRORS/constraints.json
+-rw-r--r--   0        0        0     1952 2022-08-23 13:18:42.136334 cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/import_error_1w3_IMPORT_AT_SAMPLING_STEP_WITH_ERRORS/constraints_manager.pkl
+-rw-r--r--   0        0        0      158 2022-07-29 11:03:25.478398 cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/import_error_1w3_IMPORT_AT_SAMPLING_STEP_WITH_ERRORS/metadata.json
+-rw-r--r--   0        0        0     3295 2022-07-29 11:07:16.516888 cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/import_error_1w3_IMPORT_AT_SAMPLING_STEP_WITH_ERRORS/modelization.json
+-rw-r--r--   0        0        0        2 2022-07-11 12:07:21.309471 cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/import_error_1w3_IMPORT_AT_SAMPLING_STEP_WITH_ERRORS/sampling.json
+-rw-r--r--   0        0        0     1580 2022-08-16 08:27:27.996356 cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/import_error_1w3_IMPORT_AT_SAMPLING_STEP_WITH_ERRORS/settings.json
+-rw-r--r--   0        0        0       99 2022-07-29 14:59:58.636777 cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/import_error_1w3_IMPORT_AT_SAMPLING_STEP_WITH_ERRORS/status.json
+-rw-r--r--   0        0        0     6513 2022-07-29 11:07:05.483900 cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/import_error_1w3_IMPORT_AT_SAMPLING_STEP_WITH_ERRORS/texts.json
+-rw-r--r--   0        0        0     5825 2022-07-29 11:07:06.474279 cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/import_error_1w3_IMPORT_AT_SAMPLING_STEP_WITH_ERRORS/vectors.pkl
+-rw-r--r--   0        0        0     2106 2022-07-29 11:07:12.409116 cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/import_error_1w3_IMPORT_AT_SAMPLING_STEP_WITH_ERRORS/vectors_2D.json
+-rw-r--r--   0        0        0     2904 2022-07-29 11:07:15.505121 cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/import_error_1w3_IMPORT_AT_SAMPLING_STEP_WITH_ERRORS/vectors_3D.json
+-rw-r--r--   0        0        0      444 2022-08-16 08:29:35.853846 cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/import_error_1x1_IMPORT_AT_ANNOTATION_STEP_WITH_PENDING_MODELIZATION/clustering.json
+-rw-r--r--   0        0        0     1810 2022-07-29 10:12:35.231746 cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/import_error_1x1_IMPORT_AT_ANNOTATION_STEP_WITH_PENDING_MODELIZATION/constraints.json
+-rw-r--r--   0        0        0      163 2022-07-29 10:07:25.679543 cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/import_error_1x1_IMPORT_AT_ANNOTATION_STEP_WITH_PENDING_MODELIZATION/metadata.json
+-rw-r--r--   0        0        0     3045 2022-07-11 12:07:21.303486 cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/import_error_1x1_IMPORT_AT_ANNOTATION_STEP_WITH_PENDING_MODELIZATION/modelization.json
+-rw-r--r--   0        0        0        2 2022-07-11 12:07:21.309471 cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/import_error_1x1_IMPORT_AT_ANNOTATION_STEP_WITH_PENDING_MODELIZATION/sampling.json
+-rw-r--r--   0        0        0     1580 2022-08-16 08:27:38.472320 cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/import_error_1x1_IMPORT_AT_ANNOTATION_STEP_WITH_PENDING_MODELIZATION/settings.json
+-rw-r--r--   0        0        0      209 2022-08-23 08:03:11.331549 cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/import_error_1x1_IMPORT_AT_ANNOTATION_STEP_WITH_PENDING_MODELIZATION/status.json
+-rw-r--r--   0        0        0     6513 2022-07-11 12:10:23.869094 cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/import_error_1x1_IMPORT_AT_ANNOTATION_STEP_WITH_PENDING_MODELIZATION/texts.json
+-rw-r--r--   0        0        0      444 2022-08-16 08:29:43.768715 cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/import_error_1x3_ANNOTATION_WITH_OUTDATED_MODELIZATION_WITH_CONFLICTS/clustering.json
+-rw-r--r--   0        0        0     1809 2022-07-29 11:07:37.951319 cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/import_error_1x3_ANNOTATION_WITH_OUTDATED_MODELIZATION_WITH_CONFLICTS/constraints.json
+-rw-r--r--   0        0        0     1952 2022-08-23 13:18:42.143315 cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/import_error_1x3_ANNOTATION_WITH_OUTDATED_MODELIZATION_WITH_CONFLICTS/constraints_manager.pkl
+-rw-r--r--   0        0        0      175 2022-07-29 11:03:59.823007 cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/import_error_1x3_ANNOTATION_WITH_OUTDATED_MODELIZATION_WITH_CONFLICTS/metadata.json
+-rw-r--r--   0        0        0     3295 2022-07-29 11:07:38.406161 cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/import_error_1x3_ANNOTATION_WITH_OUTDATED_MODELIZATION_WITH_CONFLICTS/modelization.json
+-rw-r--r--   0        0        0        2 2022-07-11 12:07:21.309471 cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/import_error_1x3_ANNOTATION_WITH_OUTDATED_MODELIZATION_WITH_CONFLICTS/sampling.json
+-rw-r--r--   0        0        0     1580 2022-08-16 08:27:46.098266 cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/import_error_1x3_ANNOTATION_WITH_OUTDATED_MODELIZATION_WITH_CONFLICTS/settings.json
+-rw-r--r--   0        0        0      116 2022-07-29 15:00:54.721230 cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/import_error_1x3_ANNOTATION_WITH_OUTDATED_MODELIZATION_WITH_CONFLICTS/status.json
+-rw-r--r--   0        0        0     6513 2022-07-29 11:07:35.037212 cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/import_error_1x3_ANNOTATION_WITH_OUTDATED_MODELIZATION_WITH_CONFLICTS/texts.json
+-rw-r--r--   0        0        0     5825 2022-07-29 11:07:35.496991 cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/import_error_1x3_ANNOTATION_WITH_OUTDATED_MODELIZATION_WITH_CONFLICTS/vectors.pkl
+-rw-r--r--   0        0        0     2106 2022-07-29 11:07:36.384630 cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/import_error_1x3_ANNOTATION_WITH_OUTDATED_MODELIZATION_WITH_CONFLICTS/vectors_2D.json
+-rw-r--r--   0        0        0     2904 2022-07-29 11:07:37.453644 cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/import_error_1x3_ANNOTATION_WITH_OUTDATED_MODELIZATION_WITH_CONFLICTS/vectors_3D.json
+-rw-r--r--   0        0        0      444 2022-08-16 08:29:48.698371 cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/import_error_1y1_IMPORT_AT_CLUSTERING_STEP_WITH_PENDING_MODELIZATION/clustering.json
+-rw-r--r--   0        0        0     1810 2022-07-29 10:12:35.231746 cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/import_error_1y1_IMPORT_AT_CLUSTERING_STEP_WITH_PENDING_MODELIZATION/constraints.json
+-rw-r--r--   0        0        0      163 2022-07-29 10:07:25.679543 cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/import_error_1y1_IMPORT_AT_CLUSTERING_STEP_WITH_PENDING_MODELIZATION/metadata.json
+-rw-r--r--   0        0        0     3045 2022-07-11 12:07:21.303486 cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/import_error_1y1_IMPORT_AT_CLUSTERING_STEP_WITH_PENDING_MODELIZATION/modelization.json
+-rw-r--r--   0        0        0        2 2022-07-11 12:07:21.309471 cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/import_error_1y1_IMPORT_AT_CLUSTERING_STEP_WITH_PENDING_MODELIZATION/sampling.json
+-rw-r--r--   0        0        0     1580 2022-08-16 08:27:52.228290 cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/import_error_1y1_IMPORT_AT_CLUSTERING_STEP_WITH_PENDING_MODELIZATION/settings.json
+-rw-r--r--   0        0        0      209 2022-08-23 08:03:11.325564 cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/import_error_1y1_IMPORT_AT_CLUSTERING_STEP_WITH_PENDING_MODELIZATION/status.json
+-rw-r--r--   0        0        0     6513 2022-07-11 12:10:23.869094 cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/import_error_1y1_IMPORT_AT_CLUSTERING_STEP_WITH_PENDING_MODELIZATION/texts.json
+-rw-r--r--   0        0        0        2 2022-07-11 12:07:21.312463 cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/import_error_1y3_IMPORT_AT_CLUSTERING_STEP_WITH_ERRORS/clustering.json
+-rw-r--r--   0        0        0     1809 2022-07-29 11:08:01.407612 cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/import_error_1y3_IMPORT_AT_CLUSTERING_STEP_WITH_ERRORS/constraints.json
+-rw-r--r--   0        0        0     1952 2022-08-23 13:18:42.150300 cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/import_error_1y3_IMPORT_AT_CLUSTERING_STEP_WITH_ERRORS/constraints_manager.pkl
+-rw-r--r--   0        0        0      160 2022-07-29 11:04:53.647016 cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/import_error_1y3_IMPORT_AT_CLUSTERING_STEP_WITH_ERRORS/metadata.json
+-rw-r--r--   0        0        0     3295 2022-07-29 11:08:01.848439 cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/import_error_1y3_IMPORT_AT_CLUSTERING_STEP_WITH_ERRORS/modelization.json
+-rw-r--r--   0        0        0        2 2022-07-11 12:07:21.309471 cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/import_error_1y3_IMPORT_AT_CLUSTERING_STEP_WITH_ERRORS/sampling.json
+-rw-r--r--   0        0        0     1580 2022-08-16 08:27:57.792616 cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/import_error_1y3_IMPORT_AT_CLUSTERING_STEP_WITH_ERRORS/settings.json
+-rw-r--r--   0        0        0      101 2022-07-29 15:00:30.036260 cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/import_error_1y3_IMPORT_AT_CLUSTERING_STEP_WITH_ERRORS/status.json
+-rw-r--r--   0        0        0     6513 2022-07-29 11:07:57.236796 cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/import_error_1y3_IMPORT_AT_CLUSTERING_STEP_WITH_ERRORS/texts.json
+-rw-r--r--   0        0        0     5825 2022-07-29 11:07:57.866120 cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/import_error_1y3_IMPORT_AT_CLUSTERING_STEP_WITH_ERRORS/vectors.pkl
+-rw-r--r--   0        0        0     2106 2022-07-29 11:07:58.905499 cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/import_error_1y3_IMPORT_AT_CLUSTERING_STEP_WITH_ERRORS/vectors_2D.json
+-rw-r--r--   0        0        0     2904 2022-07-29 11:08:00.851094 cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/import_error_1y3_IMPORT_AT_CLUSTERING_STEP_WITH_ERRORS/vectors_3D.json
+-rw-r--r--   0        0        0      867 2022-08-16 08:30:39.719787 cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/import_error_1z1_IMPORT_AT_ITERATION_END_WITH_PENDING_MODELIZATION/clustering.json
+-rw-r--r--   0        0        0     1810 2022-07-29 10:12:35.231746 cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/import_error_1z1_IMPORT_AT_ITERATION_END_WITH_PENDING_MODELIZATION/constraints.json
+-rw-r--r--   0        0        0      163 2022-07-29 10:07:25.679543 cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/import_error_1z1_IMPORT_AT_ITERATION_END_WITH_PENDING_MODELIZATION/metadata.json
+-rw-r--r--   0        0        0     3045 2022-07-11 12:07:21.303486 cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/import_error_1z1_IMPORT_AT_ITERATION_END_WITH_PENDING_MODELIZATION/modelization.json
+-rw-r--r--   0        0        0        2 2022-07-11 12:07:21.309471 cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/import_error_1z1_IMPORT_AT_ITERATION_END_WITH_PENDING_MODELIZATION/sampling.json
+-rw-r--r--   0        0        0     1580 2022-08-16 08:28:02.649641 cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/import_error_1z1_IMPORT_AT_ITERATION_END_WITH_PENDING_MODELIZATION/settings.json
+-rw-r--r--   0        0        0      207 2022-08-23 08:03:11.325564 cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/import_error_1z1_IMPORT_AT_ITERATION_END_WITH_PENDING_MODELIZATION/status.json
+-rw-r--r--   0        0        0     6513 2022-07-11 12:10:23.869094 cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/import_error_1z1_IMPORT_AT_ITERATION_END_WITH_PENDING_MODELIZATION/texts.json
+-rw-r--r--   0        0        0      867 2022-08-16 08:30:33.193314 cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/import_error_1z3_IMPORT_AT_ITERATION_END_WITH_ERRORS/clustering.json
+-rw-r--r--   0        0        0     1809 2022-07-29 11:08:29.596577 cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/import_error_1z3_IMPORT_AT_ITERATION_END_WITH_ERRORS/constraints.json
+-rw-r--r--   0        0        0     1952 2022-08-23 13:18:42.156284 cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/import_error_1z3_IMPORT_AT_ITERATION_END_WITH_ERRORS/constraints_manager.pkl
+-rw-r--r--   0        0        0      158 2022-07-29 11:05:26.855897 cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/import_error_1z3_IMPORT_AT_ITERATION_END_WITH_ERRORS/metadata.json
+-rw-r--r--   0        0        0     3295 2022-07-29 11:08:30.039362 cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/import_error_1z3_IMPORT_AT_ITERATION_END_WITH_ERRORS/modelization.json
+-rw-r--r--   0        0        0        2 2022-07-11 12:07:21.309471 cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/import_error_1z3_IMPORT_AT_ITERATION_END_WITH_ERRORS/sampling.json
+-rw-r--r--   0        0        0     1580 2022-08-16 08:28:08.092799 cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/import_error_1z3_IMPORT_AT_ITERATION_END_WITH_ERRORS/settings.json
+-rw-r--r--   0        0        0       99 2022-07-29 15:01:48.266216 cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/import_error_1z3_IMPORT_AT_ITERATION_END_WITH_ERRORS/status.json
+-rw-r--r--   0        0        0     6513 2022-07-29 11:08:24.466061 cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/import_error_1z3_IMPORT_AT_ITERATION_END_WITH_ERRORS/texts.json
+-rw-r--r--   0        0        0     5825 2022-07-29 11:08:24.936923 cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/import_error_1z3_IMPORT_AT_ITERATION_END_WITH_ERRORS/vectors.pkl
+-rw-r--r--   0        0        0     2106 2022-07-29 11:08:26.680342 cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/import_error_1z3_IMPORT_AT_ITERATION_END_WITH_ERRORS/vectors_2D.json
+-rw-r--r--   0        0        0     2904 2022-07-29 11:08:29.027093 cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/import_error_1z3_IMPORT_AT_ITERATION_END_WITH_ERRORS/vectors_3D.json
+-rw-r--r--   0        0        0     6115 2023-02-16 16:47:15.559515 cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies_utils.py
+-rw-r--r--   0        0        0      858 2022-08-22 15:59:06.845649 cognitivefactory-interactive-clustering-gui-0.4.1/tests/test_app.py
+-rw-r--r--   0        0        0      971 2022-08-23 07:48:17.781994 cognitivefactory-interactive-clustering-gui-0.4.1/tests/test_backgroundtasks.py
+-rw-r--r--   0        0        0     1093 2022-08-26 15:44:17.408153 cognitivefactory-interactive-clustering-gui-0.4.1/tests/test_cli.py
+-rw-r--r--   0        0        0     3230 2022-08-23 11:37:04.834986 cognitivefactory-interactive-clustering-gui-0.4.1/tests/test_delete_api_projects.py
+-rw-r--r--   0        0        0     1062 2022-07-22 13:34:01.176251 cognitivefactory-interactive-clustering-gui-0.4.1/tests/test_get_alive.py
+-rw-r--r--   0        0        0     2606 2022-07-25 14:31:40.122180 cognitivefactory-interactive-clustering-gui-0.4.1/tests/test_get_api_projects.py
+-rw-r--r--   0        0        0    10271 2022-07-26 09:10:34.242910 cognitivefactory-interactive-clustering-gui-0.4.1/tests/test_get_api_projects_clustering.py
+-rw-r--r--   0        0        0   203926 2022-08-18 15:15:28.910254 cognitivefactory-interactive-clustering-gui-0.4.1/tests/test_get_api_projects_constraints.py
+-rw-r--r--   0        0        0     4054 2022-07-25 14:53:28.619212 cognitivefactory-interactive-clustering-gui-0.4.1/tests/test_get_api_projects_download.py
+-rw-r--r--   0        0        0     3047 2022-07-28 06:34:57.853635 cognitivefactory-interactive-clustering-gui-0.4.1/tests/test_get_api_projects_metadata.py
+-rw-r--r--   0        0        0    10686 2022-07-25 14:15:53.467482 cognitivefactory-interactive-clustering-gui-0.4.1/tests/test_get_api_projects_modelization.py
+-rw-r--r--   0        0        0    18434 2022-08-18 13:29:11.062683 cognitivefactory-interactive-clustering-gui-0.4.1/tests/test_get_api_projects_sampling.py
+-rw-r--r--   0        0        0    13930 2022-08-18 13:29:08.531336 cognitivefactory-interactive-clustering-gui-0.4.1/tests/test_get_api_projects_settings.py
+-rw-r--r--   0        0        0     5411 2022-08-23 08:03:48.974293 cognitivefactory-interactive-clustering-gui-0.4.1/tests/test_get_api_projects_status.py
+-rw-r--r--   0        0        0    53392 2022-07-25 14:10:08.984923 cognitivefactory-interactive-clustering-gui-0.4.1/tests/test_get_api_projects_texts.py
+-rw-r--r--   0        0        0     9477 2022-07-27 07:14:13.049815 cognitivefactory-interactive-clustering-gui-0.4.1/tests/test_get_api_projects_vectors.py
+-rw-r--r--   0        0        0     1081 2022-07-22 13:33:57.668268 cognitivefactory-interactive-clustering-gui-0.4.1/tests/test_get_gui_help.py
+-rw-r--r--   0        0        0     7987 2022-07-26 08:01:48.258129 cognitivefactory-interactive-clustering-gui-0.4.1/tests/test_get_gui_projects_constraints.py
+-rw-r--r--   0        0        0    10312 2022-07-27 08:11:56.167878 cognitivefactory-interactive-clustering-gui-0.4.1/tests/test_get_gui_projects_constraints_annotation.py
+-rw-r--r--   0        0        0     9317 2022-07-25 14:31:40.122180 cognitivefactory-interactive-clustering-gui-0.4.1/tests/test_get_gui_projects_home.py
+-rw-r--r--   0        0        0     6789 2022-07-29 14:50:33.631265 cognitivefactory-interactive-clustering-gui-0.4.1/tests/test_get_gui_projects_listing.py
+-rw-r--r--   0        0        0    13315 2022-07-27 07:23:07.286328 cognitivefactory-interactive-clustering-gui-0.4.1/tests/test_get_gui_projects_settings.py
+-rw-r--r--   0        0        0     7706 2022-07-25 14:53:16.989570 cognitivefactory-interactive-clustering-gui-0.4.1/tests/test_get_gui_projects_texts.py
+-rw-r--r--   0        0        0      935 2022-07-25 14:57:11.394414 cognitivefactory-interactive-clustering-gui-0.4.1/tests/test_get_ready.py
+-rw-r--r--   0        0        0     1048 2022-08-31 15:09:00.725396 cognitivefactory-interactive-clustering-gui-0.4.1/tests/test_get_welcome.py
+-rw-r--r--   0        0        0    11755 2022-08-22 15:59:06.841665 cognitivefactory-interactive-clustering-gui-0.4.1/tests/test_post_api_projects.py
+-rw-r--r--   0        0        0     9996 2022-08-23 14:15:24.749320 cognitivefactory-interactive-clustering-gui-0.4.1/tests/test_post_api_projects_clustering.py
+-rw-r--r--   0        0        0    11389 2022-07-26 13:50:01.419643 cognitivefactory-interactive-clustering-gui-0.4.1/tests/test_post_api_projects_constraints_approve.py
+-rw-r--r--   0        0        0    10398 2022-07-25 14:34:47.900760 cognitivefactory-interactive-clustering-gui-0.4.1/tests/test_post_api_projects_iterations.py
+-rw-r--r--   0        0        0    24960 2022-08-24 09:11:46.541829 cognitivefactory-interactive-clustering-gui-0.4.1/tests/test_post_api_projects_modelization.py
+-rw-r--r--   0        0        0    10030 2022-08-24 09:12:45.857916 cognitivefactory-interactive-clustering-gui-0.4.1/tests/test_post_api_projects_sampling.py
+-rw-r--r--   0        0        0    24426 2022-07-25 14:52:59.709528 cognitivefactory-interactive-clustering-gui-0.4.1/tests/test_put_api_projects.py
+-rw-r--r--   0        0        0    25890 2022-07-26 13:50:01.413659 cognitivefactory-interactive-clustering-gui-0.4.1/tests/test_put_api_projects_constraints_annotate.py
+-rw-r--r--   0        0        0     9038 2022-07-26 13:50:01.415654 cognitivefactory-interactive-clustering-gui-0.4.1/tests/test_put_api_projects_constraints_comment.py
+-rw-r--r--   0        0        0    11185 2022-07-26 13:50:01.408678 cognitivefactory-interactive-clustering-gui-0.4.1/tests/test_put_api_projects_constraints_review.py
+-rw-r--r--   0        0        0    76179 2022-07-27 11:39:00.153602 cognitivefactory-interactive-clustering-gui-0.4.1/tests/test_put_api_projects_settings.py
+-rw-r--r--   0        0        0    20464 2022-07-26 13:53:12.255355 cognitivefactory-interactive-clustering-gui-0.4.1/tests/test_put_api_projects_texts_delete.py
+-rw-r--r--   0        0        0    18904 2022-07-26 13:53:26.121350 cognitivefactory-interactive-clustering-gui-0.4.1/tests/test_put_api_projects_texts_rename.py
+-rw-r--r--   0        0        0    20442 2022-07-26 13:52:57.711966 cognitivefactory-interactive-clustering-gui-0.4.1/tests/test_put_api_projects_texts_undelete.py
+-rw-r--r--   0        0        0     7155 2022-08-23 14:21:58.860410 cognitivefactory-interactive-clustering-gui-0.4.1/tests/test_run_constrained_clustering_task.py
+-rw-r--r--   0        0        0    23297 2022-08-23 14:21:58.891658 cognitivefactory-interactive-clustering-gui-0.4.1/tests/test_run_constraints_sampling_task.py
+-rw-r--r--   0        0        0   311634 2022-08-23 14:21:59.125982 cognitivefactory-interactive-clustering-gui-0.4.1/tests/test_run_modelization_update_task.py
+-rw-r--r--   0        0        0     2906 2022-08-22 17:41:44.848998 cognitivefactory-interactive-clustering-gui-0.4.1/tests/test_utils_jinja_filters.py
+-rw-r--r--   0        0        0     1193 2022-08-22 15:59:06.825664 cognitivefactory-interactive-clustering-gui-0.4.1/tests/test_utils_models_settings.py
+-rw-r--r--   0        0        0     1229 2022-08-22 15:59:06.823669 cognitivefactory-interactive-clustering-gui-0.4.1/tests/test_utils_models_states.py
+-rw-r--r--   0        0        0     6654 1970-01-01 00:00:00.000000 cognitivefactory-interactive-clustering-gui-0.4.1/PKG-INFO
```

### Comparing `cognitivefactory-interactive-clustering-gui-0.4.0/LICENSE.md` & `cognitivefactory-interactive-clustering-gui-0.4.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `cognitivefactory-interactive-clustering-gui-0.4.0/pyproject.toml` & `cognitivefactory-interactive-clustering-gui-0.4.1/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 [project]
 name = "cognitivefactory-interactive-clustering-gui"
 description = "A web application designed for NLP data annotation using Interactive Clustering methodology."
 authors = [
     { name = "Erwan Schild", email = "erwan.schild@e-i.com" },
 ]
 readme = "README.md"
-requires-python = ">=3.7"
+requires-python = ">=3.8"
 keywords = [
     "natural-language-processing",
     "constraints",
     "annotation-tool",
     "interactive-clustering",
     "constraints-annotation",
 ]
@@ -24,15 +24,14 @@
 ]
 classifiers = [
     "Development Status :: 4 - Beta",
     "Intended Audience :: Developers",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3 :: Only",
-    "Programming Language :: Python :: 3.7",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Topic :: Documentation",
     "Topic :: Software Development",
     "Topic :: Software Development :: Documentation",
     "Topic :: Utilities",
     "Typing :: Typed",
@@ -40,24 +39,23 @@
 dependencies = [
     "pandas>=1.1.4",
     "cognitivefactory-interactive-clustering>=0.5.2",
     "scikit-learn>=0.24.1",
     "fastapi>=0.65.2",
     "filelock>=3.0.12",
     "jinja2>=3.0.1",
-    "importlib-metadata>=4.8.1",
     "loguru>=0.5.3",
     "openpyxl>=3.0.7",
-    "pickle5>=0.0.12; python_version < '3.8'",
     "prometheus-fastapi-instrumentator>=5.5.1",
     "python-multipart>=0.0.5",
     "uvicorn>=0.12.2",
     "zipp>=3.5.0",
+    "setuptools>=65.5.1",
 ]
-version = "0.4.0"
+version = "0.4.1"
 
 [project.license]
 text = "CECILL-C"
 
 [project.urls]
 Homepage = "https://cognitivefactory.github.io/interactive-clustering-gui"
 Documentation = "https://cognitivefactory.github.io/interactive-clustering-gui"
@@ -79,77 +77,79 @@
 
 [tool.pdm.build]
 package-dir = "src"
 editable-backend = "editables"
 
 [tool.pdm.dev-dependencies]
 develop = [
-    "locust>=1.1",
     "fr-core-news-md @ https://github.com/explosion/spacy-models/releases/download/fr_core_news_md-3.1.0/fr_core_news_md-3.1.0.tar.gz",
 ]
 duty = [
     "duty>=0.7",
 ]
 format = [
     "autoflake>=1.4",
     "black>=21.10b0",
     "isort>=5.10",
 ]
 quality = [
+    "flake8>=4",
     "darglint>=1.8",
-    "flake8<5",
     "flake8-bandit>=2.1",
     "flake8-black>=0.2",
     "flake8-bugbear>=21.9",
     "flake8-builtins>=1.5",
     "flake8-comprehensions>=3.7",
     "flake8-docstrings>=1.6",
     "flake8-pytest-style>=1.5",
     "flake8-string-format>=0.3",
     "flake8-tidy-imports>=4.5",
     "flake8-variables-names>=0.0",
     "pep8-naming>=0.12",
     "wps-light>=0.15",
+    "gitpython>=3.1.30",
 ]
 docs = [
     "mkdocs>=1.3",
     "mkdocs-coverage>=0.2",
     "mkdocs-gen-files>=0.3",
     "mkdocs-literate-nav>=0.4",
     "mkdocs-material>=7.3",
     "mkdocs-section-index>=0.3",
     "mkdocstrings[python]>=0.19",
     "markdown-callouts>=0.2",
     "markdown-exec>=0.5",
     "toml>=0.10",
+    "certifi>=2022.12.7",
 ]
 typing = [
     "mypy>=0.910",
     "types-filelock",
     "types-markdown>=3.3",
     "types-python-dateutil",
     "types-toml>=0.10",
 ]
 security = [
-    "safety>=1.10,<2",
+    "safety>=2",
+    "certifi>=2022.12.7",
 ]
 tests = [
     "httpx>=0.16",
     "hypothesis>=6.8",
     "pytest>=6.2",
     "pytest-asyncio>=0.14",
     "pytest-cov>=3.0",
     "pytest-mock>=3.4",
     "pytest-randomly>=3.10",
     "pytest-sugar>=0.9",
     "pytest-xdist>=2.4",
     "fr-core-news-md @ https://github.com/explosion/spacy-models/releases/download/fr_core_news_md-3.1.0/fr_core_news_md-3.1.0.tar.gz",
 ]
 maintain = [
-    "git-changelog>=0.4",
+    "git-changelog>=0.4,<1.0",
 ]
 
 [tool.black]
 line-length = 120
 exclude = "tests/fixtures"
 
 [tool.isort]
```

### Comparing `cognitivefactory-interactive-clustering-gui-0.4.0/README.md` & `cognitivefactory-interactive-clustering-gui-0.4.1/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,379 +1,416 @@
-00000000: 2320 496e 7465 7261 6374 6976 6520 436c  # Interactive Cl
-00000010: 7573 7465 7269 6e67 2047 5549 0a0a 5b21  ustering GUI..[!
-00000020: 5b63 695d 2868 7474 7073 3a2f 2f67 6974  [ci](https://git
-00000030: 6875 622e 636f 6d2f 636f 676e 6974 6976  hub.com/cognitiv
-00000040: 6566 6163 746f 7279 2f69 6e74 6572 6163  efactory/interac
-00000050: 7469 7665 2d63 6c75 7374 6572 696e 672d  tive-clustering-
-00000060: 6775 692f 776f 726b 666c 6f77 732f 6369  gui/workflows/ci
-00000070: 2f62 6164 6765 2e73 7667 295d 2868 7474  /badge.svg)](htt
-00000080: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
-00000090: 636f 676e 6974 6976 6566 6163 746f 7279  cognitivefactory
-000000a0: 2f69 6e74 6572 6163 7469 7665 2d63 6c75  /interactive-clu
-000000b0: 7374 6572 696e 672d 6775 692f 6163 7469  stering-gui/acti
-000000c0: 6f6e 733f 7175 6572 793d 776f 726b 666c  ons?query=workfl
-000000d0: 6f77 2533 4163 6929 0a5b 215b 646f 6375  ow%3Aci).[![docu
-000000e0: 6d65 6e74 6174 696f 6e5d 2868 7474 7073  mentation](https
-000000f0: 3a2f 2f69 6d67 2e73 6869 656c 6473 2e69  ://img.shields.i
-00000100: 6f2f 6261 6467 652f 646f 6373 2d6d 6b64  o/badge/docs-mkd
-00000110: 6f63 7325 3230 6d61 7465 7269 616c 2d62  ocs%20material-b
-00000120: 6c75 652e 7376 673f 7374 796c 653d 666c  lue.svg?style=fl
-00000130: 6174 295d 2868 7474 7073 3a2f 2f63 6f67  at)](https://cog
-00000140: 6e69 7469 7665 6661 6374 6f72 792e 6769  nitivefactory.gi
-00000150: 7468 7562 2e69 6f2f 696e 7465 7261 6374  thub.io/interact
-00000160: 6976 652d 636c 7573 7465 7269 6e67 2d67  ive-clustering-g
-00000170: 7569 2f29 0a5b 215b 7079 7069 2076 6572  ui/).[![pypi ver
-00000180: 7369 6f6e 5d28 6874 7470 733a 2f2f 696d  sion](https://im
-00000190: 672e 7368 6965 6c64 732e 696f 2f70 7970  g.shields.io/pyp
-000001a0: 692f 762f 636f 676e 6974 6976 6566 6163  i/v/cognitivefac
-000001b0: 746f 7279 2d69 6e74 6572 6163 7469 7665  tory-interactive
-000001c0: 2d63 6c75 7374 6572 696e 672d 6775 692e  -clustering-gui.
-000001d0: 7376 6729 5d28 6874 7470 733a 2f2f 7079  svg)](https://py
-000001e0: 7069 2e6f 7267 2f70 726f 6a65 6374 2f63  pi.org/project/c
-000001f0: 6f67 6e69 7469 7665 6661 6374 6f72 792d  ognitivefactory-
-00000200: 696e 7465 7261 6374 6976 652d 636c 7573  interactive-clus
-00000210: 7465 7269 6e67 2d67 7569 2f29 0a5b 215b  tering-gui/).[![
-00000220: 444f 495d 2868 7474 7073 3a2f 2f7a 656e  DOI](https://zen
-00000230: 6f64 6f2e 6f72 672f 6261 6467 652f 444f  odo.org/badge/DO
-00000240: 492f 3130 2e35 3238 312f 7a65 6e6f 646f  I/10.5281/zenodo
-00000250: 2e34 3737 3532 3730 2e73 7667 295d 2868  .4775270.svg)](h
-00000260: 7474 7073 3a2f 2f64 6f69 2e6f 7267 2f31  ttps://doi.org/1
-00000270: 302e 3532 3831 2f7a 656e 6f64 6f2e 3437  0.5281/zenodo.47
-00000280: 3735 3237 3029 0a0a 0a41 2077 6562 2061  75270)...A web a
-00000290: 7070 6c69 6361 7469 6f6e 2064 6573 6967  pplication desig
-000002a0: 6e65 6420 666f 7220 4e4c 5020 6461 7461  ned for NLP data
-000002b0: 2061 6e6e 6f74 6174 696f 6e20 7573 696e   annotation usin
-000002c0: 6720 496e 7465 7261 6374 6976 6520 436c  g Interactive Cl
-000002d0: 7573 7465 7269 6e67 206d 6574 686f 646f  ustering methodo
-000002e0: 6c6f 6779 2e0a 0a23 2320 3c61 206e 616d  logy...## <a nam
-000002f0: 653d 2244 6573 6372 6970 7469 6f6e 223e  e="Description">
-00000300: 3c2f 613e 2051 7569 636b 2064 6573 6372  </a> Quick descr
-00000310: 6970 7469 6f6e 0a0a 5f49 6e74 6572 6163  iption.._Interac
-00000320: 7469 7665 2063 6c75 7374 6572 696e 675f  tive clustering_
-00000330: 2069 7320 6120 6d65 7468 6f64 2069 6e74   is a method int
-00000340: 656e 6465 6420 746f 2061 7373 6973 7420  ended to assist 
-00000350: 696e 2074 6865 2064 6573 6967 6e20 6f66  in the design of
-00000360: 2061 2074 7261 696e 696e 6720 6461 7461   a training data
-00000370: 2073 6574 2e0a 0a54 6869 7320 6974 6572   set...This iter
-00000380: 6174 6976 6520 7072 6f63 6573 7320 6265  ative process be
-00000390: 6769 6e73 2077 6974 6820 616e 2075 6e6c  gins with an unl
-000003a0: 6162 656c 6564 2064 6174 6173 6574 2c20  abeled dataset, 
-000003b0: 616e 6420 6974 2075 7365 7320 6120 7365  and it uses a se
-000003c0: 7175 656e 6365 206f 6620 7477 6f20 7375  quence of two su
-000003d0: 6273 7465 7073 203a 0a0a 312e 2074 6865  bsteps :..1. the
-000003e0: 2075 7365 7220 6465 6669 6e65 7320 636f   user defines co
-000003f0: 6e73 7472 6169 6e74 7320 6f6e 2064 6174  nstraints on dat
-00000400: 6120 7361 6d70 6c65 6420 6279 2074 6865  a sampled by the
-00000410: 2063 6f6d 7075 7465 7220 3b0a 322e 2074   computer ;.2. t
-00000420: 6865 2063 6f6d 7075 7465 7220 7065 7266  he computer perf
-00000430: 6f72 6d73 2064 6174 6120 7061 7274 6974  orms data partit
-00000440: 696f 6e69 6e67 2075 7369 6e67 2061 2063  ioning using a c
-00000450: 6f6e 7374 7261 696e 6564 2063 6c75 7374  onstrained clust
-00000460: 6572 696e 6720 616c 676f 7269 7468 6d2e  ering algorithm.
-00000470: 0a0a 5468 7573 2c20 6174 2065 6163 6820  ..Thus, at each 
-00000480: 7374 6570 206f 6620 7468 6520 7072 6f63  step of the proc
-00000490: 6573 7320 3a0a 0a2d 2074 6865 2075 7365  ess :..- the use
-000004a0: 7220 636f 7272 6563 7473 2074 6865 2063  r corrects the c
-000004b0: 6c75 7374 6572 696e 6720 6f66 2074 6865  lustering of the
-000004c0: 2070 7265 7669 6f75 7320 7374 6570 7320   previous steps 
-000004d0: 7573 696e 6720 636f 6e73 7472 6169 6e74  using constraint
-000004e0: 732c 2061 6e64 0a2d 2074 6865 2063 6f6d  s, and.- the com
-000004f0: 7075 7465 7220 6f66 6665 7273 2061 2063  puter offers a c
-00000500: 6f72 7265 6374 6564 2061 6e64 206d 6f72  orrected and mor
-00000510: 6520 7265 6c65 7661 6e74 2064 6174 6120  e relevant data 
-00000520: 7061 7274 6974 696f 6e69 6e67 2066 6f72  partitioning for
-00000530: 2074 6865 206e 6578 7420 7374 6570 2e0a   the next step..
-00000540: 0a54 6869 7320 7765 6220 6170 706c 6963  .This web applic
-00000550: 6174 696f 6e20 696d 706c 656d 656e 7473  ation implements
-00000560: 2074 6869 7320 616e 6e6f 7461 7469 6f6e   this annotation
-00000570: 206d 6574 686f 646f 6c6f 6779 2077 6974   methodology wit
-00000580: 6820 7365 7665 7261 6c20 6665 6174 7572  h several featur
-00000590: 6573 3a0a 0a2d 205f 6461 7461 2070 7265  es:..- _data pre
-000005a0: 7072 6f63 6573 7369 6e67 2061 6e64 2076  processing and v
-000005b0: 6563 746f 7269 7a61 7469 6f6e 5f20 696e  ectorization_ in
-000005c0: 206f 7264 6572 2074 6f20 7265 6475 6365   order to reduce
-000005d0: 206e 6f69 7365 2069 6e20 6461 7461 3b0a   noise in data;.
-000005e0: 2d20 5f63 6f6e 7374 7261 696e 7465 6420  - _constrainted 
-000005f0: 636c 7573 7465 7269 6e67 5f20 696e 206f  clustering_ in o
-00000600: 7264 6572 2074 6f20 6175 746f 6d61 7469  rder to automati
-00000610: 6361 6c6c 7920 7061 7274 6974 696f 6e20  cally partition 
-00000620: 7468 6520 6461 7461 3b0a 2d20 5f63 6f6e  the data;.- _con
-00000630: 7374 7261 696e 7473 2073 616d 706c 696e  straints samplin
-00000640: 675f 2069 6e20 6f72 6465 7220 746f 2073  g_ in order to s
-00000650: 656c 6563 7420 7468 6520 6d6f 7374 2072  elect the most r
-00000660: 656c 6576 616e 7420 6461 7461 2074 6f20  elevant data to 
-00000670: 616e 6e6f 7461 7465 3b0a 2d20 5f62 696e  annotate;.- _bin
-00000680: 6172 7920 636f 6e73 7472 6169 6e74 7320  ary constraints 
-00000690: 616e 6e6f 7461 7469 6f6e 5f20 696e 206f  annotation_ in o
-000006a0: 7264 6572 2074 6f20 636f 7272 6563 7420  rder to correct 
-000006b0: 636c 7573 7465 7269 6e67 2072 656c 6576  clustering relev
-000006c0: 616e 6365 3b0a 2d20 5f61 6e6e 6f74 6174  ance;.- _annotat
-000006d0: 696f 6e20 7265 7669 6577 2061 6e64 2063  ion review and c
-000006e0: 6f6e 666c 6963 7473 2061 6e61 6c79 7369  onflicts analysi
-000006f0: 735f 2069 6e20 6f72 6465 7220 746f 2069  s_ in order to i
-00000700: 6d70 726f 7665 2063 6f6e 7374 7261 696e  mprove constrain
-00000710: 7473 2063 6f6e 7369 7374 656e 6379 2e0a  ts consistency..
-00000720: 0a46 6f72 206d 6f72 6520 6465 7461 696c  .For more detail
-00000730: 732c 2072 6561 6420 7468 6520 5b44 6f63  s, read the [Doc
-00000740: 756d 656e 7461 7469 6f6e 5d28 2344 6f63  umentation](#Doc
-00000750: 756d 656e 7461 7469 6f6e 2920 616e 6420  umentation) and 
-00000760: 7468 6520 6172 7469 636c 6573 2069 6e20  the articles in 
-00000770: 7468 6520 5b52 6566 6572 656e 6365 735d  the [References]
-00000780: 2823 5265 6665 7265 6e63 6573 2920 7365  (#References) se
-00000790: 6374 696f 6e2e 0a0a 2323 203c 6120 6e61  ction...## <a na
-000007a0: 6d65 3d22 446f 6375 6d65 6e74 6174 696f  me="Documentatio
-000007b0: 6e22 3e3c 2f61 3e20 446f 6375 6d65 6e74  n"></a> Document
-000007c0: 6174 696f 6e0a 0a2d 205b 4d61 696e 2064  ation..- [Main d
-000007d0: 6f63 756d 656e 7461 7469 6f6e 5d28 6874  ocumentation](ht
-000007e0: 7470 733a 2f2f 636f 676e 6974 6976 6566  tps://cognitivef
-000007f0: 6163 746f 7279 2e67 6974 6875 622e 696f  actory.github.io
-00000800: 2f69 6e74 6572 6163 7469 7665 2d63 6c75  /interactive-clu
-00000810: 7374 6572 696e 672d 6775 692f 290a 0a23  stering-gui/)..#
-00000820: 2320 3c61 206e 616d 653d 2252 6571 7569  # <a name="Requi
-00000830: 7265 6d65 6e74 7322 3e3c 2f61 3e20 5265  rements"></a> Re
-00000840: 7175 6972 656d 656e 7473 0a0a 496e 7465  quirements..Inte
-00000850: 7261 6374 6976 6520 436c 7573 7465 7269  ractive Clusteri
-00000860: 6e67 2047 5549 2072 6571 7569 7265 7320  ng GUI requires 
-00000870: 5079 7468 6f6e 2033 2e37 206f 7220 6162  Python 3.7 or ab
-00000880: 6f76 652e 0a0a 3c64 6574 6169 6c73 3e0a  ove...<details>.
-00000890: 3c73 756d 6d61 7279 3e54 6f20 696e 7374  <summary>To inst
-000008a0: 616c 6c20 5079 7468 6f6e 2033 2e37 2c20  all Python 3.7, 
-000008b0: 4920 7265 636f 6d6d 656e 6420 7573 696e  I recommend usin
-000008c0: 6720 3c61 2068 7265 663d 2268 7474 7073  g <a href="https
-000008d0: 3a2f 2f67 6974 6875 622e 636f 6d2f 7079  ://github.com/py
-000008e0: 656e 762f 7079 656e 7622 3e3c 636f 6465  env/pyenv"><code
-000008f0: 3e70 7965 6e76 3c2f 636f 6465 3e3c 2f61  >pyenv</code></a
-00000900: 3e2e 3c2f 7375 6d6d 6172 793e 0a0a 6060  >.</summary>..``
-00000910: 6062 6173 680a 2320 696e 7374 616c 6c20  `bash.# install 
-00000920: 7079 656e 760a 6769 7420 636c 6f6e 6520  pyenv.git clone 
-00000930: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
-00000940: 6f6d 2f70 7965 6e76 2f70 7965 6e76 207e  om/pyenv/pyenv ~
-00000950: 2f2e 7079 656e 760a 0a23 2073 6574 7570  /.pyenv..# setup
-00000960: 2070 7965 6e76 2028 796f 7520 7368 6f75   pyenv (you shou
-00000970: 6c64 2061 6c73 6f20 7075 7420 7468 6573  ld also put thes
-00000980: 6520 7468 7265 6520 6c69 6e65 7320 696e  e three lines in
-00000990: 202e 6261 7368 7263 206f 7220 7369 6d69   .bashrc or simi
-000009a0: 6c61 7229 0a65 7870 6f72 7420 5041 5448  lar).export PATH
-000009b0: 3d22 247b 484f 4d45 7d2f 2e70 7965 6e76  ="${HOME}/.pyenv
-000009c0: 2f62 696e 3a24 7b50 4154 487d 220a 6578  /bin:${PATH}".ex
-000009d0: 706f 7274 2050 5945 4e56 5f52 4f4f 543d  port PYENV_ROOT=
-000009e0: 2224 7b48 4f4d 457d 2f2e 7079 656e 7622  "${HOME}/.pyenv"
-000009f0: 0a65 7661 6c20 2224 2870 7965 6e76 2069  .eval "$(pyenv i
-00000a00: 6e69 7420 2d29 220a 0a23 2069 6e73 7461  nit -)"..# insta
-00000a10: 6c6c 2050 7974 686f 6e20 332e 370a 7079  ll Python 3.7.py
-00000a20: 656e 7620 696e 7374 616c 6c20 332e 370a  env install 3.7.
-00000a30: 0a23 206d 616b 6520 6974 2061 7661 696c  .# make it avail
-00000a40: 6162 6c65 2067 6c6f 6261 6c6c 790a 7079  able globally.py
-00000a50: 656e 7620 676c 6f62 616c 2073 7973 7465  env global syste
-00000a60: 6d20 332e 370a 6060 600a 3c2f 6465 7461  m 3.7.```.</deta
-00000a70: 696c 733e 0a0a 2323 203c 6120 6e61 6d65  ils>..## <a name
-00000a80: 3d22 496e 7374 616c 6c61 7469 6f6e 223e  ="Installation">
-00000a90: 3c2f 613e 2049 6e73 7461 6c6c 6174 696f  </a> Installatio
-00000aa0: 6e0a 0a57 6974 6820 6070 6970 603a 0a60  n..With `pip`:.`
-00000ab0: 6060 6261 7368 0a23 2069 6e73 7461 6c6c  ``bash.# install
-00000ac0: 2070 6163 6b61 6765 0a70 7974 686f 6e33   package.python3
-00000ad0: 202d 6d20 7069 7020 696e 7374 616c 6c20   -m pip install 
-00000ae0: 636f 676e 6974 6976 6566 6163 746f 7279  cognitivefactory
-00000af0: 2d69 6e74 6572 6163 7469 7665 2d63 6c75  -interactive-clu
-00000b00: 7374 6572 696e 672d 6775 690a 0a23 2069  stering-gui..# i
-00000b10: 6e73 7461 6c6c 2073 7061 6379 206c 616e  nstall spacy lan
-00000b20: 6775 6167 6520 6d6f 6465 6c20 6465 7065  guage model depe
-00000b30: 6e64 656e 6369 6573 2028 7468 6520 6f6e  ndencies (the on
-00000b40: 6520 796f 7520 7761 6e74 2c20 7769 7468  e you want, with
-00000b50: 2076 6572 7369 6f6e 2022 332e 312e 7822   version "3.1.x"
-00000b60: 290a 7079 7468 6f6e 3320 2d6d 2073 7061  ).python3 -m spa
-00000b70: 6379 2064 6f77 6e6c 6f61 6420 6672 5f63  cy download fr_c
-00000b80: 6f72 655f 6e65 7773 5f6d 642d 332e 312e  ore_news_md-3.1.
-00000b90: 3020 2d2d 6469 7265 6374 0a60 6060 0a0a  0 --direct.```..
-00000ba0: 5769 7468 205b 6070 6970 7860 5d28 6874  With [`pipx`](ht
-00000bb0: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
-00000bc0: 2f70 6970 7870 726f 6a65 6374 2f70 6970  /pipxproject/pip
-00000bd0: 7829 3a0a 6060 6062 6173 680a 2320 696e  x):.```bash.# in
-00000be0: 7374 616c 6c20 7069 7078 0a70 7974 686f  stall pipx.pytho
-00000bf0: 6e33 202d 6d20 7069 7020 696e 7374 616c  n3 -m pip instal
-00000c00: 6c20 2d2d 7573 6572 2070 6970 780a 0a23  l --user pipx..#
-00000c10: 2069 6e73 7461 6c6c 2070 6163 6b61 6765   install package
-00000c20: 0a70 6970 7820 696e 7374 616c 6c20 2d2d  .pipx install --
-00000c30: 7079 7468 6f6e 2070 7974 686f 6e33 2063  python python3 c
-00000c40: 6f67 6e69 7469 7665 6661 6374 6f72 792d  ognitivefactory-
-00000c50: 696e 7465 7261 6374 6976 652d 636c 7573  interactive-clus
-00000c60: 7465 7269 6e67 2d67 7569 0a0a 2320 696e  tering-gui..# in
-00000c70: 7374 616c 6c20 7370 6163 7920 6c61 6e67  stall spacy lang
-00000c80: 7561 6765 206d 6f64 656c 2064 6570 656e  uage model depen
-00000c90: 6465 6e63 6965 7320 2874 6865 206f 6e65  dencies (the one
-00000ca0: 2079 6f75 2077 616e 742c 2077 6974 6820   you want, with 
-00000cb0: 7665 7273 696f 6e20 2233 2e31 2e78 2229  version "3.1.x")
-00000cc0: 0a70 7974 686f 6e33 202d 6d20 7370 6163  .python3 -m spac
-00000cd0: 7920 646f 776e 6c6f 6164 2066 725f 636f  y download fr_co
-00000ce0: 7265 5f6e 6577 735f 6d64 2d33 2e31 2e30  re_news_md-3.1.0
-00000cf0: 202d 2d64 6972 6563 740a 6060 600a 0a23   --direct.```..#
-00000d00: 2320 3c61 206e 616d 653d 2252 756e 223e  # <a name="Run">
-00000d10: 3c2f 613e 2052 756e 0a0a 546f 2064 6973  </a> Run..To dis
-00000d20: 706c 6179 2074 6865 2068 656c 7020 6d65  play the help me
-00000d30: 7373 6167 653a 0a0a 6060 6062 6173 680a  ssage:..```bash.
-00000d40: 636f 676e 6974 6976 6566 6163 746f 7279  cognitivefactory
-00000d50: 2d69 6e74 6572 6163 7469 7665 2d63 6c75  -interactive-clu
-00000d60: 7374 6572 696e 672d 6775 6920 2d2d 6865  stering-gui --he
-00000d70: 6c70 0a60 6060 0a0a 546f 206c 6175 6e63  lp.```..To launc
-00000d80: 6820 7468 6520 7765 6220 6170 706c 6963  h the web applic
-00000d90: 6174 696f 6e3a 0a0a 6060 6062 6173 680a  ation:..```bash.
-00000da0: 636f 676e 6974 6976 6566 6163 746f 7279  cognitivefactory
-00000db0: 2d69 6e74 6572 6163 7469 7665 2d63 6c75  -interactive-clu
-00000dc0: 7374 6572 696e 672d 6775 6920 2023 206c  stering-gui  # l
-00000dd0: 6175 6e63 6820 6f6e 2031 3237 2e30 2e30  aunch on 127.0.0
-00000de0: 2e31 3a38 3038 300a 6060 600a 0a54 6865  .1:8080.```..The
-00000df0: 6e2c 2067 6f20 746f 206f 6e65 206f 6620  n, go to one of 
-00000e00: 7468 6520 666f 6c6c 6f77 696e 6720 7061  the following pa
-00000e10: 6765 7320 696e 2079 6f75 7220 6272 6f77  ges in your brow
-00000e20: 7365 723a 0a0a 2d20 5765 6c63 6f6d 6520  ser:..- Welcome 
-00000e30: 7061 6765 2028 7765 6220 6170 706c 6963  page (web applic
-00000e40: 6174 696f 6e20 686f 6d65 293a 205b 6874  ation home): [ht
-00000e50: 7470 3a2f 2f6c 6f63 616c 686f 7374 3a38  tp://localhost:8
-00000e60: 3038 305d 2868 7474 703a 2f2f 6c6f 6361  080](http://loca
-00000e70: 6c68 6f73 743a 3830 3830 290a 2d20 5377  lhost:8080).- Sw
-00000e80: 6167 6765 7220 2869 6e74 6572 6163 7469  agger (interacti
-00000e90: 7665 2064 6f63 756d 656e 7461 7469 6f6e  ve documentation
-00000ea0: 293a 205b 6874 7470 3a2f 2f6c 6f63 616c  ): [http://local
-00000eb0: 686f 7374 3a38 3038 302f 646f 6373 5d28  host:8080/docs](
-00000ec0: 6874 7470 3a2f 2f6c 6f63 616c 686f 7374  http://localhost
-00000ed0: 3a38 3038 302f 646f 6373 290a 0a23 2320  :8080/docs)..## 
-00000ee0: 3c61 206e 616d 653d 2244 6576 656c 6f70  <a name="Develop
-00000ef0: 6d65 6e74 223e 3c2f 613e 2044 6576 656c  ment"></a> Devel
-00000f00: 6f70 6d65 6e74 0a0a 546f 2077 6f72 6b20  opment..To work 
-00000f10: 6f6e 2074 6869 7320 7072 6f6a 6563 7420  on this project 
-00000f20: 6f72 2063 6f6e 7472 6962 7574 6520 746f  or contribute to
-00000f30: 2069 742c 2070 6c65 6173 6520 7265 6164   it, please read
-00000f40: 0a5b 7468 6520 436f 7069 6572 2050 444d  .[the Copier PDM
-00000f50: 2064 6f63 756d 656e 7461 7469 6f6e 5d28   documentation](
-00000f60: 6874 7470 733a 2f2f 7061 7761 6d6f 792e  https://pawamoy.
-00000f70: 6769 7468 7562 2e69 6f2f 636f 7069 6572  github.io/copier
-00000f80: 2d70 646d 2f29 2e0a 0a23 2323 2051 7569  -pdm/)...### Qui
-00000f90: 636b 2073 6574 7570 2061 6e64 2068 656c  ck setup and hel
-00000fa0: 700a 0a47 6574 2074 6865 2063 6f64 6520  p..Get the code 
-00000fb0: 616e 6420 7072 6570 6172 6520 7468 6520  and prepare the 
-00000fc0: 656e 7669 726f 6e6d 656e 743a 0a0a 6060  environment:..``
-00000fd0: 6062 6173 680a 6769 7420 636c 6f6e 6520  `bash.git clone 
-00000fe0: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
-00000ff0: 6f6d 2f63 6f67 6e69 7469 7665 6661 6374  om/cognitivefact
-00001000: 6f72 792f 696e 7465 7261 6374 6976 652d  ory/interactive-
-00001010: 636c 7573 7465 7269 6e67 2d67 7569 2f0a  clustering-gui/.
-00001020: 6364 2069 6e74 6572 6163 7469 7665 2d63  cd interactive-c
-00001030: 6c75 7374 6572 696e 672d 6775 690a 6d61  lustering-gui.ma
-00001040: 6b65 2073 6574 7570 0a60 6060 0a0a 5368  ke setup.```..Sh
-00001050: 6f77 2074 6865 2068 656c 703a 0a0a 6060  ow the help:..``
-00001060: 6062 6173 680a 6d61 6b65 2068 656c 7020  `bash.make help 
-00001070: 2023 206f 7220 6a75 7374 206d 616b 650a   # or just make.
-00001080: 6060 600a 0a4c 6175 6e63 6820 7468 6520  ```..Launch the 
-00001090: 7765 6220 6170 706c 6963 6174 696f 6e20  web application 
-000010a0: 696e 2064 6562 7567 206d 6f64 653a 0a0a  in debug mode:..
-000010b0: 6060 6062 6173 680a 6d61 6b65 2072 756e  ```bash.make run
-000010c0: 2020 2320 6c61 756e 6368 206f 6e20 3132    # launch on 12
-000010d0: 372e 302e 302e 313a 3830 3830 0a60 6060  7.0.0.1:8080.```
-000010e0: 0a0a 5468 656e 2c20 676f 2074 6f20 6f6e  ..Then, go to on
-000010f0: 6520 6f66 2074 6865 2066 6f6c 6c6f 7769  e of the followi
-00001100: 6e67 2070 6167 6573 2069 6e20 796f 7572  ng pages in your
-00001110: 2062 726f 7773 6572 3a0a 0a2d 2057 656c   browser:..- Wel
-00001120: 636f 6d65 2070 6167 6520 2877 6562 2061  come page (web a
-00001130: 7070 6c69 6361 7469 6f6e 2068 6f6d 6529  pplication home)
-00001140: 3a20 5b68 7474 703a 2f2f 6c6f 6361 6c68  : [http://localh
-00001150: 6f73 743a 3830 3830 5d28 6874 7470 3a2f  ost:8080](http:/
-00001160: 2f6c 6f63 616c 686f 7374 3a38 3038 3029  /localhost:8080)
-00001170: 0a2d 2053 7761 6767 6572 2028 696e 7465  .- Swagger (inte
-00001180: 7261 6374 6976 6520 646f 6375 6d65 6e74  ractive document
-00001190: 6174 696f 6e29 3a20 5b68 7474 703a 2f2f  ation): [http://
-000011a0: 6c6f 6361 6c68 6f73 743a 3830 3830 2f64  localhost:8080/d
-000011b0: 6f63 735d 2868 7474 703a 2f2f 6c6f 6361  ocs](http://loca
-000011c0: 6c68 6f73 743a 3830 3830 2f64 6f63 7329  lhost:8080/docs)
-000011d0: 0a0a 466f 7220 6d6f 7265 2064 6574 6169  ..For more detai
-000011e0: 6c73 2c20 7265 6164 2074 6865 205b 436f  ls, read the [Co
-000011f0: 6e74 7269 6275 7469 6e67 5d28 6874 7470  ntributing](http
-00001200: 733a 2f2f 636f 676e 6974 6976 6566 6163  s://cognitivefac
-00001210: 746f 7279 2e67 6974 6875 622e 696f 2f69  tory.github.io/i
-00001220: 6e74 6572 6163 7469 7665 2d63 6c75 7374  nteractive-clust
-00001230: 6572 696e 672d 6775 692f 636f 6e74 7269  ering-gui/contri
-00001240: 6275 7469 6e67 2f29 2064 6f63 756d 656e  buting/) documen
-00001250: 7461 7469 6f6e 2e0a 0a23 2320 3c61 206e  tation...## <a n
-00001260: 616d 653d 2252 6566 6572 656e 6365 7322  ame="References"
-00001270: 3e3c 2f61 3e20 5265 6665 7265 6e63 6573  ></a> References
-00001280: 0a0a 2d20 2a2a 496e 7465 7261 6374 6976  ..- **Interactiv
-00001290: 6520 436c 7573 7465 7269 6e67 2a2a 3a0a  e Clustering**:.
-000012a0: 2020 2020 2d20 4669 7273 7420 7072 6573      - First pres
-000012b0: 656e 7461 7469 6f6e 3a20 6053 6368 696c  entation: `Schil
-000012c0: 642c 2045 2e2c 2044 7572 616e 7469 6e2c  d, E., Durantin,
-000012d0: 2047 2e2c 204c 616d 6972 656c 2c20 4a2e   G., Lamirel, J.
-000012e0: 432e 2c20 2620 4d69 636f 6e69 2c20 462e  C., & Miconi, F.
-000012f0: 2028 3230 3231 292e 2043 6f6e 6365 7074   (2021). Concept
-00001300: 696f 6e20 6974 c3a9 7261 7469 7665 2065  ion it..rative e
-00001310: 7420 7365 6d69 2d73 7570 6572 7669 73c3  t semi-supervis.
-00001320: a965 2064 2761 7373 6973 7461 6e74 7320  .e d'assistants 
-00001330: 636f 6e76 6572 7361 7469 6f6e 6e65 6c73  conversationnels
-00001340: 2070 6172 2072 6567 726f 7570 656d 656e   par regroupemen
-00001350: 7420 696e 7465 7261 6374 6966 2064 6573  t interactif des
-00001360: 2071 7565 7374 696f 6e73 2e20 496e 2045   questions. In E
-00001370: 4743 2032 3032 3120 2d20 3231 c3a8 6d65  GC 2021 - 21..me
-00001380: 7320 4a6f 7572 6ec3 a965 7320 4672 616e  s Journ..es Fran
-00001390: 636f 7068 6f6e 6573 2045 7874 7261 6374  cophones Extract
-000013a0: 696f 6e20 6574 2047 6573 7469 6f6e 2064  ion et Gestion d
-000013b0: 6573 2043 6f6e 6e61 6973 7361 6e63 6573  es Connaissances
-000013c0: 2e20 4564 6974 696f 6e20 524e 5449 2e20  . Edition RNTI. 
-000013d0: e29f a868 616c 2d30 3331 3333 3030 37e2  ...hal-03133007.
-000013e0: 9fa9 2e60 0a20 2020 202d 2054 6865 6f72  ...`.    - Theor
-000013f0: 6574 6963 616c 2073 7475 6479 3a20 6053  etical study: `S
-00001400: 6368 696c 642c 2045 2e2c 2044 7572 616e  child, E., Duran
-00001410: 7469 6e2c 2047 2e2c 204c 616d 6972 656c  tin, G., Lamirel
-00001420: 2c20 4a2e 2c20 2620 4d69 636f 6e69 2c20  , J., & Miconi, 
-00001430: 462e 2028 3230 3232 292e 2049 7465 7261  F. (2022). Itera
-00001440: 7469 7665 2061 6e64 2053 656d 692d 5375  tive and Semi-Su
-00001450: 7065 7276 6973 6564 2044 6573 6967 6e20  pervised Design 
-00001460: 6f66 2043 6861 7462 6f74 7320 5573 696e  of Chatbots Usin
-00001470: 6720 496e 7465 7261 6374 6976 6520 436c  g Interactive Cl
-00001480: 7573 7465 7269 6e67 2e20 496e 7465 726e  ustering. Intern
-00001490: 6174 696f 6e61 6c20 4a6f 7572 6e61 6c20  ational Journal 
-000014a0: 6f66 2044 6174 6120 5761 7265 686f 7573  of Data Warehous
-000014b0: 696e 6720 616e 6420 4d69 6e69 6e67 2028  ing and Mining (
-000014c0: 494a 4457 4d29 2c20 3138 2832 292c 2031  IJDWM), 18(2), 1
-000014d0: 2d31 392e 2068 7474 703a 2f2f 646f 692e  -19. http://doi.
-000014e0: 6f72 672f 3130 2e34 3031 382f 494a 4457  org/10.4018/IJDW
-000014f0: 4d2e 3239 3830 3037 2e20 e29f a868 616c  M.298007. ...hal
-00001500: 2d30 3336 3438 3034 31e2 9fa9 2e60 0a20  -03648041....`. 
-00001510: 2020 202d 204d 6574 686f 646f 6c6f 6769     - Methodologi
-00001520: 6361 6c20 6469 7363 7573 7369 6f6e 3a20  cal discussion: 
-00001530: 6053 6368 696c 642c 2045 2e2c 2044 7572  `Schild, E., Dur
-00001540: 616e 7469 6e2c 2047 2e2c 2026 204c 616d  antin, G., & Lam
-00001550: 6972 656c 2c20 4a2e 432e 2028 3230 3231  irel, J.C. (2021
-00001560: 292e 2043 6f6e 6365 766f 6972 2075 6e20  ). Concevoir un 
-00001570: 6173 7369 7374 616e 7420 636f 6e76 6572  assistant conver
-00001580: 7361 7469 6f6e 6e65 6c20 6465 206d 616e  sationnel de man
-00001590: 69c3 a872 6520 6974 c3a9 7261 7469 7665  i..re it..rative
-000015a0: 2065 7420 7365 6d69 2d73 7570 6572 7669   et semi-supervi
-000015b0: 73c3 a965 2061 7665 6320 6c65 2063 6c75  s..e avec le clu
-000015c0: 7374 6572 696e 6720 696e 7465 7261 6374  stering interact
-000015d0: 6966 2e20 496e 2041 7465 6c69 6572 202d  if. In Atelier -
-000015e0: 2046 6f75 696c 6c65 2064 6520 5465 7874   Fouille de Text
-000015f0: 6573 202d 2054 6578 7420 4d69 6e65 2032  es - Text Mine 2
-00001600: 3032 3120 2d20 456e 2063 6f6e 6a6f 6e63  021 - En conjonc
-00001610: 7469 6f6e 2061 7665 6320 4547 4320 3230  tion avec EGC 20
-00001620: 3231 2e20 e29f a868 616c 2d30 3331 3333  21. ...hal-03133
-00001630: 3036 30e2 9fa9 2e60 0a20 2020 202d 2049  060....`.    - I
-00001640: 6d70 6c65 6d65 6e74 6174 696f 6e3a 2060  mplementation: `
-00001650: 5363 6869 6c64 2c20 452e 2028 3230 3231  Schild, E. (2021
-00001660: 292e 2063 6f67 6e69 7469 7665 6661 6374  ). cognitivefact
-00001670: 6f72 792f 696e 7465 7261 6374 6976 652d  ory/interactive-
-00001680: 636c 7573 7465 7269 6e67 2e20 5a65 6e6f  clustering. Zeno
-00001690: 646f 2e20 6874 7470 733a 2f2f 646f 692e  do. https://doi.
-000016a0: 6f72 672f 3130 2e35 3238 312f 7a65 6e6f  org/10.5281/zeno
-000016b0: 646f 2e34 3737 3532 3531 2e60 0a0a 2d20  do.4775251.`..- 
-000016c0: 2a2a 5765 6220 6170 706c 6963 6174 696f  **Web applicatio
-000016d0: 6e2a 2a3a 0a20 2020 202d 205f 4661 7374  n**:.    - _Fast
-000016e0: 4150 495f 3a20 6068 7474 7073 3a2f 2f66  API_: `https://f
-000016f0: 6173 7461 7069 2e74 6961 6e67 6f6c 6f2e  astapi.tiangolo.
-00001700: 636f 6d2f 600a 0a23 2320 3c61 206e 616d  com/`..## <a nam
-00001710: 653d 2248 6f77 2074 6f20 6369 7465 223e  e="How to cite">
-00001720: 3c2f 613e 2048 6f77 2074 6f20 6369 7465  </a> How to cite
-00001730: 0a0a 6053 6368 696c 642c 2045 2e20 2832  ..`Schild, E. (2
-00001740: 3032 3129 2e20 636f 676e 6974 6976 6566  021). cognitivef
-00001750: 6163 746f 7279 2f69 6e74 6572 6163 7469  actory/interacti
-00001760: 7665 2d63 6c75 7374 6572 696e 672d 6775  ve-clustering-gu
-00001770: 692e 205a 656e 6f64 6f2e 2068 7474 7073  i. Zenodo. https
-00001780: 3a2f 2f64 6f69 2e6f 7267 2f31 302e 3532  ://doi.org/10.52
-00001790: 3831 2f7a 656e 6f64 6f2e 3437 3735 3237  81/zenodo.477527
-000017a0: 302e 60                                  0.`
+00000000: 4d65 7461 6461 7461 2d56 6572 7369 6f6e  Metadata-Version
+00000010: 3a20 322e 310a 4e61 6d65 3a20 636f 676e  : 2.1.Name: cogn
+00000020: 6974 6976 6566 6163 746f 7279 2d69 6e74  itivefactory-int
+00000030: 6572 6163 7469 7665 2d63 6c75 7374 6572  eractive-cluster
+00000040: 696e 672d 6775 690a 5665 7273 696f 6e3a  ing-gui.Version:
+00000050: 2030 2e34 2e31 0a53 756d 6d61 7279 3a20   0.4.1.Summary: 
+00000060: 4120 7765 6220 6170 706c 6963 6174 696f  A web applicatio
+00000070: 6e20 6465 7369 676e 6564 2066 6f72 204e  n designed for N
+00000080: 4c50 2064 6174 6120 616e 6e6f 7461 7469  LP data annotati
+00000090: 6f6e 2075 7369 6e67 2049 6e74 6572 6163  on using Interac
+000000a0: 7469 7665 2043 6c75 7374 6572 696e 6720  tive Clustering 
+000000b0: 6d65 7468 6f64 6f6c 6f67 792e 0a4c 6963  methodology..Lic
+000000c0: 656e 7365 3a20 4345 4349 4c4c 2d43 0a4b  ense: CECILL-C.K
+000000d0: 6579 776f 7264 733a 206e 6174 7572 616c  eywords: natural
+000000e0: 2d6c 616e 6775 6167 652d 7072 6f63 6573  -language-proces
+000000f0: 7369 6e67 2c63 6f6e 7374 7261 696e 7473  sing,constraints
+00000100: 2c61 6e6e 6f74 6174 696f 6e2d 746f 6f6c  ,annotation-tool
+00000110: 2c69 6e74 6572 6163 7469 7665 2d63 6c75  ,interactive-clu
+00000120: 7374 6572 696e 672c 636f 6e73 7472 6169  stering,constrai
+00000130: 6e74 732d 616e 6e6f 7461 7469 6f6e 0a41  nts-annotation.A
+00000140: 7574 686f 722d 656d 6169 6c3a 2045 7277  uthor-email: Erw
+00000150: 616e 2053 6368 696c 6420 3c65 7277 616e  an Schild <erwan
+00000160: 2e73 6368 696c 6440 652d 692e 636f 6d3e  .schild@e-i.com>
+00000170: 0a52 6571 7569 7265 732d 5079 7468 6f6e  .Requires-Python
+00000180: 3a20 3e3d 332e 380a 436c 6173 7369 6669  : >=3.8.Classifi
+00000190: 6572 3a20 4465 7665 6c6f 706d 656e 7420  er: Development 
+000001a0: 5374 6174 7573 203a 3a20 3420 2d20 4265  Status :: 4 - Be
+000001b0: 7461 0a43 6c61 7373 6966 6965 723a 2049  ta.Classifier: I
+000001c0: 6e74 656e 6465 6420 4175 6469 656e 6365  ntended Audience
+000001d0: 203a 3a20 4465 7665 6c6f 7065 7273 0a43   :: Developers.C
+000001e0: 6c61 7373 6966 6965 723a 2050 726f 6772  lassifier: Progr
+000001f0: 616d 6d69 6e67 204c 616e 6775 6167 6520  amming Language 
+00000200: 3a3a 2050 7974 686f 6e0a 436c 6173 7369  :: Python.Classi
+00000210: 6669 6572 3a20 5072 6f67 7261 6d6d 696e  fier: Programmin
+00000220: 6720 4c61 6e67 7561 6765 203a 3a20 5079  g Language :: Py
+00000230: 7468 6f6e 203a 3a20 330a 436c 6173 7369  thon :: 3.Classi
+00000240: 6669 6572 3a20 5072 6f67 7261 6d6d 696e  fier: Programmin
+00000250: 6720 4c61 6e67 7561 6765 203a 3a20 5079  g Language :: Py
+00000260: 7468 6f6e 203a 3a20 3320 3a3a 204f 6e6c  thon :: 3 :: Onl
+00000270: 790a 436c 6173 7369 6669 6572 3a20 5072  y.Classifier: Pr
+00000280: 6f67 7261 6d6d 696e 6720 4c61 6e67 7561  ogramming Langua
+00000290: 6765 203a 3a20 5079 7468 6f6e 203a 3a20  ge :: Python :: 
+000002a0: 332e 380a 436c 6173 7369 6669 6572 3a20  3.8.Classifier: 
+000002b0: 5072 6f67 7261 6d6d 696e 6720 4c61 6e67  Programming Lang
+000002c0: 7561 6765 203a 3a20 5079 7468 6f6e 203a  uage :: Python :
+000002d0: 3a20 332e 390a 436c 6173 7369 6669 6572  : 3.9.Classifier
+000002e0: 3a20 546f 7069 6320 3a3a 2044 6f63 756d  : Topic :: Docum
+000002f0: 656e 7461 7469 6f6e 0a43 6c61 7373 6966  entation.Classif
+00000300: 6965 723a 2054 6f70 6963 203a 3a20 536f  ier: Topic :: So
+00000310: 6674 7761 7265 2044 6576 656c 6f70 6d65  ftware Developme
+00000320: 6e74 0a43 6c61 7373 6966 6965 723a 2054  nt.Classifier: T
+00000330: 6f70 6963 203a 3a20 536f 6674 7761 7265  opic :: Software
+00000340: 2044 6576 656c 6f70 6d65 6e74 203a 3a20   Development :: 
+00000350: 446f 6375 6d65 6e74 6174 696f 6e0a 436c  Documentation.Cl
+00000360: 6173 7369 6669 6572 3a20 546f 7069 6320  assifier: Topic 
+00000370: 3a3a 2055 7469 6c69 7469 6573 0a43 6c61  :: Utilities.Cla
+00000380: 7373 6966 6965 723a 2054 7970 696e 6720  ssifier: Typing 
+00000390: 3a3a 2054 7970 6564 0a50 726f 6a65 6374  :: Typed.Project
+000003a0: 2d55 524c 3a20 4368 616e 6765 6c6f 672c  -URL: Changelog,
+000003b0: 2068 7474 7073 3a2f 2f63 6f67 6e69 7469   https://cogniti
+000003c0: 7665 6661 6374 6f72 792e 6769 7468 7562  vefactory.github
+000003d0: 2e69 6f2f 696e 7465 7261 6374 6976 652d  .io/interactive-
+000003e0: 636c 7573 7465 7269 6e67 2d67 7569 2f63  clustering-gui/c
+000003f0: 6861 6e67 656c 6f67 0a50 726f 6a65 6374  hangelog.Project
+00000400: 2d55 524c 3a20 4469 7363 7573 7369 6f6e  -URL: Discussion
+00000410: 732c 2068 7474 7073 3a2f 2f67 6974 6875  s, https://githu
+00000420: 622e 636f 6d2f 636f 676e 6974 6976 6566  b.com/cognitivef
+00000430: 6163 746f 7279 2f69 6e74 6572 6163 7469  actory/interacti
+00000440: 7665 2d63 6c75 7374 6572 696e 672d 6775  ve-clustering-gu
+00000450: 692f 6469 7363 7573 7369 6f6e 730a 5072  i/discussions.Pr
+00000460: 6f6a 6563 742d 5552 4c3a 2044 6f63 756d  oject-URL: Docum
+00000470: 656e 7461 7469 6f6e 2c20 6874 7470 733a  entation, https:
+00000480: 2f2f 636f 676e 6974 6976 6566 6163 746f  //cognitivefacto
+00000490: 7279 2e67 6974 6875 622e 696f 2f69 6e74  ry.github.io/int
+000004a0: 6572 6163 7469 7665 2d63 6c75 7374 6572  eractive-cluster
+000004b0: 696e 672d 6775 690a 5072 6f6a 6563 742d  ing-gui.Project-
+000004c0: 5552 4c3a 2048 6f6d 6570 6167 652c 2068  URL: Homepage, h
+000004d0: 7474 7073 3a2f 2f63 6f67 6e69 7469 7665  ttps://cognitive
+000004e0: 6661 6374 6f72 792e 6769 7468 7562 2e69  factory.github.i
+000004f0: 6f2f 696e 7465 7261 6374 6976 652d 636c  o/interactive-cl
+00000500: 7573 7465 7269 6e67 2d67 7569 0a50 726f  ustering-gui.Pro
+00000510: 6a65 6374 2d55 524c 3a20 4973 7375 6573  ject-URL: Issues
+00000520: 2c20 6874 7470 733a 2f2f 6769 7468 7562  , https://github
+00000530: 2e63 6f6d 2f63 6f67 6e69 7469 7665 6661  .com/cognitivefa
+00000540: 6374 6f72 792f 696e 7465 7261 6374 6976  ctory/interactiv
+00000550: 652d 636c 7573 7465 7269 6e67 2d67 7569  e-clustering-gui
+00000560: 2f69 7373 7565 730a 5072 6f6a 6563 742d  /issues.Project-
+00000570: 5552 4c3a 2052 6570 6f73 6974 6f72 792c  URL: Repository,
+00000580: 2068 7474 7073 3a2f 2f67 6974 6875 622e   https://github.
+00000590: 636f 6d2f 636f 676e 6974 6976 6566 6163  com/cognitivefac
+000005a0: 746f 7279 2f69 6e74 6572 6163 7469 7665  tory/interactive
+000005b0: 2d63 6c75 7374 6572 696e 672d 6775 690a  -clustering-gui.
+000005c0: 4465 7363 7269 7074 696f 6e2d 436f 6e74  Description-Cont
+000005d0: 656e 742d 5479 7065 3a20 7465 7874 2f6d  ent-Type: text/m
+000005e0: 6172 6b64 6f77 6e0a 0a23 2049 6e74 6572  arkdown..# Inter
+000005f0: 6163 7469 7665 2043 6c75 7374 6572 696e  active Clusterin
+00000600: 6720 4755 490a 0a5b 215b 6369 5d28 6874  g GUI..[![ci](ht
+00000610: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
+00000620: 2f63 6f67 6e69 7469 7665 6661 6374 6f72  /cognitivefactor
+00000630: 792f 696e 7465 7261 6374 6976 652d 636c  y/interactive-cl
+00000640: 7573 7465 7269 6e67 2d67 7569 2f77 6f72  ustering-gui/wor
+00000650: 6b66 6c6f 7773 2f63 692f 6261 6467 652e  kflows/ci/badge.
+00000660: 7376 6729 5d28 6874 7470 733a 2f2f 6769  svg)](https://gi
+00000670: 7468 7562 2e63 6f6d 2f63 6f67 6e69 7469  thub.com/cogniti
+00000680: 7665 6661 6374 6f72 792f 696e 7465 7261  vefactory/intera
+00000690: 6374 6976 652d 636c 7573 7465 7269 6e67  ctive-clustering
+000006a0: 2d67 7569 2f61 6374 696f 6e73 3f71 7565  -gui/actions?que
+000006b0: 7279 3d77 6f72 6b66 6c6f 7725 3341 6369  ry=workflow%3Aci
+000006c0: 290a 5b21 5b64 6f63 756d 656e 7461 7469  ).[![documentati
+000006d0: 6f6e 5d28 6874 7470 733a 2f2f 696d 672e  on](https://img.
+000006e0: 7368 6965 6c64 732e 696f 2f62 6164 6765  shields.io/badge
+000006f0: 2f64 6f63 732d 6d6b 646f 6373 2532 306d  /docs-mkdocs%20m
+00000700: 6174 6572 6961 6c2d 626c 7565 2e73 7667  aterial-blue.svg
+00000710: 3f73 7479 6c65 3d66 6c61 7429 5d28 6874  ?style=flat)](ht
+00000720: 7470 733a 2f2f 636f 676e 6974 6976 6566  tps://cognitivef
+00000730: 6163 746f 7279 2e67 6974 6875 622e 696f  actory.github.io
+00000740: 2f69 6e74 6572 6163 7469 7665 2d63 6c75  /interactive-clu
+00000750: 7374 6572 696e 672d 6775 692f 290a 5b21  stering-gui/).[!
+00000760: 5b70 7970 6920 7665 7273 696f 6e5d 2868  [pypi version](h
+00000770: 7474 7073 3a2f 2f69 6d67 2e73 6869 656c  ttps://img.shiel
+00000780: 6473 2e69 6f2f 7079 7069 2f76 2f63 6f67  ds.io/pypi/v/cog
+00000790: 6e69 7469 7665 6661 6374 6f72 792d 696e  nitivefactory-in
+000007a0: 7465 7261 6374 6976 652d 636c 7573 7465  teractive-cluste
+000007b0: 7269 6e67 2d67 7569 2e73 7667 295d 2868  ring-gui.svg)](h
+000007c0: 7474 7073 3a2f 2f70 7970 692e 6f72 672f  ttps://pypi.org/
+000007d0: 7072 6f6a 6563 742f 636f 676e 6974 6976  project/cognitiv
+000007e0: 6566 6163 746f 7279 2d69 6e74 6572 6163  efactory-interac
+000007f0: 7469 7665 2d63 6c75 7374 6572 696e 672d  tive-clustering-
+00000800: 6775 692f 290a 5b21 5b44 4f49 5d28 6874  gui/).[![DOI](ht
+00000810: 7470 733a 2f2f 7a65 6e6f 646f 2e6f 7267  tps://zenodo.org
+00000820: 2f62 6164 6765 2f44 4f49 2f31 302e 3532  /badge/DOI/10.52
+00000830: 3831 2f7a 656e 6f64 6f2e 3437 3735 3237  81/zenodo.477527
+00000840: 302e 7376 6729 5d28 6874 7470 733a 2f2f  0.svg)](https://
+00000850: 646f 692e 6f72 672f 3130 2e35 3238 312f  doi.org/10.5281/
+00000860: 7a65 6e6f 646f 2e34 3737 3532 3730 290a  zenodo.4775270).
+00000870: 0a41 2077 6562 2061 7070 6c69 6361 7469  .A web applicati
+00000880: 6f6e 2064 6573 6967 6e65 6420 666f 7220  on designed for 
+00000890: 4e4c 5020 6461 7461 2061 6e6e 6f74 6174  NLP data annotat
+000008a0: 696f 6e20 7573 696e 6720 496e 7465 7261  ion using Intera
+000008b0: 6374 6976 6520 436c 7573 7465 7269 6e67  ctive Clustering
+000008c0: 206d 6574 686f 646f 6c6f 6779 2e0a 0a0a   methodology....
+000008d0: 2323 203c 6120 6e61 6d65 3d22 4465 7363  ## <a name="Desc
+000008e0: 7269 7074 696f 6e22 3e3c 2f61 3e20 5175  ription"></a> Qu
+000008f0: 6963 6b20 6465 7363 7269 7074 696f 6e0a  ick description.
+00000900: 0a5f 496e 7465 7261 6374 6976 6520 636c  ._Interactive cl
+00000910: 7573 7465 7269 6e67 5f20 6973 2061 206d  ustering_ is a m
+00000920: 6574 686f 6420 696e 7465 6e64 6564 2074  ethod intended t
+00000930: 6f20 6173 7369 7374 2069 6e20 7468 6520  o assist in the 
+00000940: 6465 7369 676e 206f 6620 6120 7472 6169  design of a trai
+00000950: 6e69 6e67 2064 6174 6120 7365 742e 0a0a  ning data set...
+00000960: 5468 6973 2069 7465 7261 7469 7665 2070  This iterative p
+00000970: 726f 6365 7373 2062 6567 696e 7320 7769  rocess begins wi
+00000980: 7468 2061 6e20 756e 6c61 6265 6c65 6420  th an unlabeled 
+00000990: 6461 7461 7365 742c 2061 6e64 2069 7420  dataset, and it 
+000009a0: 7573 6573 2061 2073 6571 7565 6e63 6520  uses a sequence 
+000009b0: 6f66 2074 776f 2073 7562 7374 6570 7320  of two substeps 
+000009c0: 3a0a 0a31 2e20 7468 6520 7573 6572 2064  :..1. the user d
+000009d0: 6566 696e 6573 2063 6f6e 7374 7261 696e  efines constrain
+000009e0: 7473 206f 6e20 6461 7461 2073 616d 706c  ts on data sampl
+000009f0: 6564 2062 7920 7468 6520 636f 6d70 7574  ed by the comput
+00000a00: 6572 203b 0a32 2e20 7468 6520 636f 6d70  er ;.2. the comp
+00000a10: 7574 6572 2070 6572 666f 726d 7320 6461  uter performs da
+00000a20: 7461 2070 6172 7469 7469 6f6e 696e 6720  ta partitioning 
+00000a30: 7573 696e 6720 6120 636f 6e73 7472 6169  using a constrai
+00000a40: 6e65 6420 636c 7573 7465 7269 6e67 2061  ned clustering a
+00000a50: 6c67 6f72 6974 686d 2e0a 0a54 6875 732c  lgorithm...Thus,
+00000a60: 2061 7420 6561 6368 2073 7465 7020 6f66   at each step of
+00000a70: 2074 6865 2070 726f 6365 7373 203a 0a0a   the process :..
+00000a80: 2d20 7468 6520 7573 6572 2063 6f72 7265  - the user corre
+00000a90: 6374 7320 7468 6520 636c 7573 7465 7269  cts the clusteri
+00000aa0: 6e67 206f 6620 7468 6520 7072 6576 696f  ng of the previo
+00000ab0: 7573 2073 7465 7073 2075 7369 6e67 2063  us steps using c
+00000ac0: 6f6e 7374 7261 696e 7473 2c20 616e 640a  onstraints, and.
+00000ad0: 2d20 7468 6520 636f 6d70 7574 6572 206f  - the computer o
+00000ae0: 6666 6572 7320 6120 636f 7272 6563 7465  ffers a correcte
+00000af0: 6420 616e 6420 6d6f 7265 2072 656c 6576  d and more relev
+00000b00: 616e 7420 6461 7461 2070 6172 7469 7469  ant data partiti
+00000b10: 6f6e 696e 6720 666f 7220 7468 6520 6e65  oning for the ne
+00000b20: 7874 2073 7465 702e 0a0a 5468 6973 2077  xt step...This w
+00000b30: 6562 2061 7070 6c69 6361 7469 6f6e 2069  eb application i
+00000b40: 6d70 6c65 6d65 6e74 7320 7468 6973 2061  mplements this a
+00000b50: 6e6e 6f74 6174 696f 6e20 6d65 7468 6f64  nnotation method
+00000b60: 6f6c 6f67 7920 7769 7468 2073 6576 6572  ology with sever
+00000b70: 616c 2066 6561 7475 7265 733a 0a0a 2d20  al features:..- 
+00000b80: 5f64 6174 6120 7072 6570 726f 6365 7373  _data preprocess
+00000b90: 696e 6720 616e 6420 7665 6374 6f72 697a  ing and vectoriz
+00000ba0: 6174 696f 6e5f 2069 6e20 6f72 6465 7220  ation_ in order 
+00000bb0: 746f 2072 6564 7563 6520 6e6f 6973 6520  to reduce noise 
+00000bc0: 696e 2064 6174 613b 0a2d 205f 636f 6e73  in data;.- _cons
+00000bd0: 7472 6169 6e74 6564 2063 6c75 7374 6572  trainted cluster
+00000be0: 696e 675f 2069 6e20 6f72 6465 7220 746f  ing_ in order to
+00000bf0: 2061 7574 6f6d 6174 6963 616c 6c79 2070   automatically p
+00000c00: 6172 7469 7469 6f6e 2074 6865 2064 6174  artition the dat
+00000c10: 613b 0a2d 205f 636f 6e73 7472 6169 6e74  a;.- _constraint
+00000c20: 7320 7361 6d70 6c69 6e67 5f20 696e 206f  s sampling_ in o
+00000c30: 7264 6572 2074 6f20 7365 6c65 6374 2074  rder to select t
+00000c40: 6865 206d 6f73 7420 7265 6c65 7661 6e74  he most relevant
+00000c50: 2064 6174 6120 746f 2061 6e6e 6f74 6174   data to annotat
+00000c60: 653b 0a2d 205f 6269 6e61 7279 2063 6f6e  e;.- _binary con
+00000c70: 7374 7261 696e 7473 2061 6e6e 6f74 6174  straints annotat
+00000c80: 696f 6e5f 2069 6e20 6f72 6465 7220 746f  ion_ in order to
+00000c90: 2063 6f72 7265 6374 2063 6c75 7374 6572   correct cluster
+00000ca0: 696e 6720 7265 6c65 7661 6e63 653b 0a2d  ing relevance;.-
+00000cb0: 205f 616e 6e6f 7461 7469 6f6e 2072 6576   _annotation rev
+00000cc0: 6965 7720 616e 6420 636f 6e66 6c69 6374  iew and conflict
+00000cd0: 7320 616e 616c 7973 6973 5f20 696e 206f  s analysis_ in o
+00000ce0: 7264 6572 2074 6f20 696d 7072 6f76 6520  rder to improve 
+00000cf0: 636f 6e73 7472 6169 6e74 7320 636f 6e73  constraints cons
+00000d00: 6973 7465 6e63 792e 0a0a 466f 7220 6d6f  istency...For mo
+00000d10: 7265 2064 6574 6169 6c73 2c20 7265 6164  re details, read
+00000d20: 2074 6865 205b 446f 6375 6d65 6e74 6174   the [Documentat
+00000d30: 696f 6e5d 2823 446f 6375 6d65 6e74 6174  ion](#Documentat
+00000d40: 696f 6e29 2061 6e64 2074 6865 2061 7274  ion) and the art
+00000d50: 6963 6c65 7320 696e 2074 6865 205b 5265  icles in the [Re
+00000d60: 6665 7265 6e63 6573 5d28 2352 6566 6572  ferences](#Refer
+00000d70: 656e 6365 7329 2073 6563 7469 6f6e 2e0a  ences) section..
+00000d80: 0a0a 2323 203c 6120 6e61 6d65 3d22 446f  ..## <a name="Do
+00000d90: 6375 6d65 6e74 6174 696f 6e22 3e3c 2f61  cumentation"></a
+00000da0: 3e20 446f 6375 6d65 6e74 6174 696f 6e0a  > Documentation.
+00000db0: 0a2d 205b 4d61 696e 2064 6f63 756d 656e  .- [Main documen
+00000dc0: 7461 7469 6f6e 5d28 6874 7470 733a 2f2f  tation](https://
+00000dd0: 636f 676e 6974 6976 6566 6163 746f 7279  cognitivefactory
+00000de0: 2e67 6974 6875 622e 696f 2f69 6e74 6572  .github.io/inter
+00000df0: 6163 7469 7665 2d63 6c75 7374 6572 696e  active-clusterin
+00000e00: 672d 6775 692f 290a 0a0a 2323 203c 6120  g-gui/)...## <a 
+00000e10: 6e61 6d65 3d22 5265 7175 6972 656d 656e  name="Requiremen
+00000e20: 7473 223e 3c2f 613e 2052 6571 7569 7265  ts"></a> Require
+00000e30: 6d65 6e74 730a 0a49 6e74 6572 6163 7469  ments..Interacti
+00000e40: 7665 2043 6c75 7374 6572 696e 6720 4755  ve Clustering GU
+00000e50: 4920 7265 7175 6972 6573 2050 7974 686f  I requires Pytho
+00000e60: 6e20 332e 3820 6f72 2061 626f 7665 2e0a  n 3.8 or above..
+00000e70: 0a54 6f20 696e 7374 616c 6c20 7769 7468  .To install with
+00000e80: 205b 6070 6970 605d 2868 7474 7073 3a2f   [`pip`](https:/
+00000e90: 2f67 6974 6875 622e 636f 6d2f 7079 7061  /github.com/pypa
+00000ea0: 2f70 6970 293a 0a0a 6060 6062 6173 680a  /pip):..```bash.
+00000eb0: 2320 696e 7374 616c 6c20 7061 636b 6167  # install packag
+00000ec0: 650a 7079 7468 6f6e 3320 2d6d 2070 6970  e.python3 -m pip
+00000ed0: 2069 6e73 7461 6c6c 2063 6f67 6e69 7469   install cogniti
+00000ee0: 7665 6661 6374 6f72 792d 696e 7465 7261  vefactory-intera
+00000ef0: 6374 6976 652d 636c 7573 7465 7269 6e67  ctive-clustering
+00000f00: 2d67 7569 0a0a 2320 696e 7374 616c 6c20  -gui..# install 
+00000f10: 7370 6163 7920 6c61 6e67 7561 6765 206d  spacy language m
+00000f20: 6f64 656c 2064 6570 656e 6465 6e63 6965  odel dependencie
+00000f30: 7320 2874 6865 206f 6e65 2079 6f75 2077  s (the one you w
+00000f40: 616e 742c 2077 6974 6820 7665 7273 696f  ant, with versio
+00000f50: 6e20 2233 2e31 2e78 2229 0a70 7974 686f  n "3.1.x").pytho
+00000f60: 6e33 202d 6d20 7370 6163 7920 646f 776e  n3 -m spacy down
+00000f70: 6c6f 6164 2066 725f 636f 7265 5f6e 6577  load fr_core_new
+00000f80: 735f 6d64 2d33 2e31 2e30 202d 2d64 6972  s_md-3.1.0 --dir
+00000f90: 6563 740a 6060 600a 0a54 6f20 696e 7374  ect.```..To inst
+00000fa0: 616c 6c20 7769 7468 205b 6070 6970 7860  all with [`pipx`
+00000fb0: 5d28 6874 7470 733a 2f2f 6769 7468 7562  ](https://github
+00000fc0: 2e63 6f6d 2f70 7970 612f 7069 7078 293a  .com/pypa/pipx):
+00000fd0: 0a0a 6060 6062 6173 680a 2320 696e 7374  ..```bash.# inst
+00000fe0: 616c 6c20 7069 7078 0a70 7974 686f 6e33  all pipx.python3
+00000ff0: 202d 6d20 7069 7020 696e 7374 616c 6c20   -m pip install 
+00001000: 2d2d 7573 6572 2070 6970 780a 0a23 2069  --user pipx..# i
+00001010: 6e73 7461 6c6c 2070 6163 6b61 6765 0a70  nstall package.p
+00001020: 6970 7820 696e 7374 616c 6c20 2d2d 7079  ipx install --py
+00001030: 7468 6f6e 2070 7974 686f 6e33 2063 6f67  thon python3 cog
+00001040: 6e69 7469 7665 6661 6374 6f72 792d 696e  nitivefactory-in
+00001050: 7465 7261 6374 6976 652d 636c 7573 7465  teractive-cluste
+00001060: 7269 6e67 2d67 7569 0a0a 2320 696e 7374  ring-gui..# inst
+00001070: 616c 6c20 7370 6163 7920 6c61 6e67 7561  all spacy langua
+00001080: 6765 206d 6f64 656c 2064 6570 656e 6465  ge model depende
+00001090: 6e63 6965 7320 2874 6865 206f 6e65 2079  ncies (the one y
+000010a0: 6f75 2077 616e 742c 2077 6974 6820 7665  ou want, with ve
+000010b0: 7273 696f 6e20 2233 2e31 2e78 2229 0a70  rsion "3.1.x").p
+000010c0: 7974 686f 6e33 202d 6d20 7370 6163 7920  ython3 -m spacy 
+000010d0: 646f 776e 6c6f 6164 2066 725f 636f 7265  download fr_core
+000010e0: 5f6e 6577 735f 6d64 2d33 2e31 2e30 202d  _news_md-3.1.0 -
+000010f0: 2d64 6972 6563 740a 6060 600a 0a0a 2323  -direct.```...##
+00001100: 203c 6120 6e61 6d65 3d22 5275 6e22 3e3c   <a name="Run"><
+00001110: 2f61 3e20 5275 6e0a 0a54 6f20 6469 7370  /a> Run..To disp
+00001120: 6c61 7920 7468 6520 6865 6c70 206d 6573  lay the help mes
+00001130: 7361 6765 3a0a 0a60 6060 6261 7368 0a63  sage:..```bash.c
+00001140: 6f67 6e69 7469 7665 6661 6374 6f72 792d  ognitivefactory-
+00001150: 696e 7465 7261 6374 6976 652d 636c 7573  interactive-clus
+00001160: 7465 7269 6e67 2d67 7569 202d 2d68 656c  tering-gui --hel
+00001170: 700a 6060 600a 0a54 6f20 6c61 756e 6368  p.```..To launch
+00001180: 2074 6865 2077 6562 2061 7070 6c69 6361   the web applica
+00001190: 7469 6f6e 3a0a 0a60 6060 6261 7368 0a63  tion:..```bash.c
+000011a0: 6f67 6e69 7469 7665 6661 6374 6f72 792d  ognitivefactory-
+000011b0: 696e 7465 7261 6374 6976 652d 636c 7573  interactive-clus
+000011c0: 7465 7269 6e67 2d67 7569 2020 2320 6c61  tering-gui  # la
+000011d0: 756e 6368 206f 6e20 3132 372e 302e 302e  unch on 127.0.0.
+000011e0: 313a 3830 3830 0a60 6060 0a0a 5468 656e  1:8080.```..Then
+000011f0: 2c20 676f 2074 6f20 6f6e 6520 6f66 2074  , go to one of t
+00001200: 6865 2066 6f6c 6c6f 7769 6e67 2070 6167  he following pag
+00001210: 6573 2069 6e20 796f 7572 2062 726f 7773  es in your brows
+00001220: 6572 3a0a 0a2d 2057 656c 636f 6d65 2070  er:..- Welcome p
+00001230: 6167 6520 2877 6562 2061 7070 6c69 6361  age (web applica
+00001240: 7469 6f6e 2068 6f6d 6529 3a20 5b68 7474  tion home): [htt
+00001250: 703a 2f2f 6c6f 6361 6c68 6f73 743a 3830  p://localhost:80
+00001260: 3830 5d28 6874 7470 3a2f 2f6c 6f63 616c  80](http://local
+00001270: 686f 7374 3a38 3038 3029 0a2d 2053 7761  host:8080).- Swa
+00001280: 6767 6572 2028 696e 7465 7261 6374 6976  gger (interactiv
+00001290: 6520 646f 6375 6d65 6e74 6174 696f 6e29  e documentation)
+000012a0: 3a20 5b68 7474 703a 2f2f 6c6f 6361 6c68  : [http://localh
+000012b0: 6f73 743a 3830 3830 2f64 6f63 735d 2868  ost:8080/docs](h
+000012c0: 7474 703a 2f2f 6c6f 6361 6c68 6f73 743a  ttp://localhost:
+000012d0: 3830 3830 2f64 6f63 7329 0a0a 0a23 2320  8080/docs)...## 
+000012e0: 3c61 206e 616d 653d 2244 6576 656c 6f70  <a name="Develop
+000012f0: 6d65 6e74 223e 3c2f 613e 2044 6576 656c  ment"></a> Devel
+00001300: 6f70 6d65 6e74 0a0a 0a54 6f20 776f 726b  opment...To work
+00001310: 206f 6e20 7468 6973 2070 726f 6a65 6374   on this project
+00001320: 206f 7220 636f 6e74 7269 6275 7465 2074   or contribute t
+00001330: 6f20 6974 2c20 706c 6561 7365 2072 6561  o it, please rea
+00001340: 643a 0a0a 2d20 7468 6520 5b43 6f70 6965  d:..- the [Copie
+00001350: 7220 5044 4d5d 2868 7474 7073 3a2f 2f70  r PDM](https://p
+00001360: 6177 616d 6f79 2e67 6974 6875 622e 696f  awamoy.github.io
+00001370: 2f63 6f70 6965 722d 7064 6d2f 2920 7465  /copier-pdm/) te
+00001380: 6d70 6c61 7465 2064 6f63 756d 656e 7461  mplate documenta
+00001390: 7469 6f6e 203b 0a2d 2074 6865 205b 436f  tion ;.- the [Co
+000013a0: 6e74 7269 6275 7469 6e67 5d28 6874 7470  ntributing](http
+000013b0: 733a 2f2f 636f 676e 6974 6976 6566 6163  s://cognitivefac
+000013c0: 746f 7279 2e67 6974 6875 622e 696f 2f69  tory.github.io/i
+000013d0: 6e74 6572 6163 7469 7665 2d63 6c75 7374  nteractive-clust
+000013e0: 6572 696e 672d 6775 692f 636f 6e74 7269  ering-gui/contri
+000013f0: 6275 7469 6e67 2f29 2070 6167 6520 666f  buting/) page fo
+00001400: 7220 656e 7669 726f 6e6d 656e 7420 7365  r environment se
+00001410: 7475 7020 616e 6420 6465 7665 6c6f 706d  tup and developm
+00001420: 656e 7420 6865 6c70 203b 0a2d 2074 6865  ent help ;.- the
+00001430: 205b 436f 6465 206f 6620 436f 6e64 7563   [Code of Conduc
+00001440: 745d 2868 7474 7073 3a2f 2f63 6f67 6e69  t](https://cogni
+00001450: 7469 7665 6661 6374 6f72 792e 6769 7468  tivefactory.gith
+00001460: 7562 2e69 6f2f 696e 7465 7261 6374 6976  ub.io/interactiv
+00001470: 652d 636c 7573 7465 7269 6e67 2d67 7569  e-clustering-gui
+00001480: 2f63 6f64 655f 6f66 5f63 6f6e 6475 6374  /code_of_conduct
+00001490: 2f29 2070 6167 6520 666f 7220 636f 6e74  /) page for cont
+000014a0: 7269 6275 7469 6f6e 2072 756c 6573 2e0a  ribution rules..
+000014b0: 0a0a 2323 203c 6120 6e61 6d65 3d22 5265  ..## <a name="Re
+000014c0: 6665 7265 6e63 6573 223e 3c2f 613e 2052  ferences"></a> R
+000014d0: 6566 6572 656e 6365 730a 0a2d 202a 2a49  eferences..- **I
+000014e0: 6e74 6572 6163 7469 7665 2043 6c75 7374  nteractive Clust
+000014f0: 6572 696e 672a 2a3a 0a20 2020 202d 2046  ering**:.    - F
+00001500: 6972 7374 2070 7265 7365 6e74 6174 696f  irst presentatio
+00001510: 6e3a 2060 5363 6869 6c64 2c20 452e 2c20  n: `Schild, E., 
+00001520: 4475 7261 6e74 696e 2c20 472e 2c20 4c61  Durantin, G., La
+00001530: 6d69 7265 6c2c 204a 2e43 2e2c 2026 204d  mirel, J.C., & M
+00001540: 6963 6f6e 692c 2046 2e20 2832 3032 3129  iconi, F. (2021)
+00001550: 2e20 436f 6e63 6570 7469 6f6e 2069 74c3  . Conception it.
+00001560: a972 6174 6976 6520 6574 2073 656d 692d  .rative et semi-
+00001570: 7375 7065 7276 6973 c3a9 6520 6427 6173  supervis..e d'as
+00001580: 7369 7374 616e 7473 2063 6f6e 7665 7273  sistants convers
+00001590: 6174 696f 6e6e 656c 7320 7061 7220 7265  ationnels par re
+000015a0: 6772 6f75 7065 6d65 6e74 2069 6e74 6572  groupement inter
+000015b0: 6163 7469 6620 6465 7320 7175 6573 7469  actif des questi
+000015c0: 6f6e 732e 2049 6e20 4547 4320 3230 3231  ons. In EGC 2021
+000015d0: 202d 2032 31c3 a86d 6573 204a 6f75 726e   - 21..mes Journ
+000015e0: c3a9 6573 2046 7261 6e63 6f70 686f 6e65  ..es Francophone
+000015f0: 7320 4578 7472 6163 7469 6f6e 2065 7420  s Extraction et 
+00001600: 4765 7374 696f 6e20 6465 7320 436f 6e6e  Gestion des Conn
+00001610: 6169 7373 616e 6365 732e 2045 6469 7469  aissances. Editi
+00001620: 6f6e 2052 4e54 492e 20e2 9fa8 6861 6c2d  on RNTI. ...hal-
+00001630: 3033 3133 3330 3037 e29f a92e 600a 2020  03133007....`.  
+00001640: 2020 2d20 5468 656f 7265 7469 6361 6c20    - Theoretical 
+00001650: 7374 7564 793a 2060 5363 6869 6c64 2c20  study: `Schild, 
+00001660: 452e 2c20 4475 7261 6e74 696e 2c20 472e  E., Durantin, G.
+00001670: 2c20 4c61 6d69 7265 6c2c 204a 2e2c 2026  , Lamirel, J., &
+00001680: 204d 6963 6f6e 692c 2046 2e20 2832 3032   Miconi, F. (202
+00001690: 3229 2e20 4974 6572 6174 6976 6520 616e  2). Iterative an
+000016a0: 6420 5365 6d69 2d53 7570 6572 7669 7365  d Semi-Supervise
+000016b0: 6420 4465 7369 676e 206f 6620 4368 6174  d Design of Chat
+000016c0: 626f 7473 2055 7369 6e67 2049 6e74 6572  bots Using Inter
+000016d0: 6163 7469 7665 2043 6c75 7374 6572 696e  active Clusterin
+000016e0: 672e 2049 6e74 6572 6e61 7469 6f6e 616c  g. International
+000016f0: 204a 6f75 726e 616c 206f 6620 4461 7461   Journal of Data
+00001700: 2057 6172 6568 6f75 7369 6e67 2061 6e64   Warehousing and
+00001710: 204d 696e 696e 6720 2849 4a44 574d 292c   Mining (IJDWM),
+00001720: 2031 3828 3229 2c20 312d 3139 2e20 6874   18(2), 1-19. ht
+00001730: 7470 3a2f 2f64 6f69 2e6f 7267 2f31 302e  tp://doi.org/10.
+00001740: 3430 3138 2f49 4a44 574d 2e32 3938 3030  4018/IJDWM.29800
+00001750: 372e 20e2 9fa8 6861 6c2d 3033 3634 3830  7. ...hal-036480
+00001760: 3431 e29f a92e 600a 2020 2020 2d20 4d65  41....`.    - Me
+00001770: 7468 6f64 6f6c 6f67 6963 616c 2064 6973  thodological dis
+00001780: 6375 7373 696f 6e3a 2060 5363 6869 6c64  cussion: `Schild
+00001790: 2c20 452e 2c20 4475 7261 6e74 696e 2c20  , E., Durantin, 
+000017a0: 472e 2c20 2620 4c61 6d69 7265 6c2c 204a  G., & Lamirel, J
+000017b0: 2e43 2e20 2832 3032 3129 2e20 436f 6e63  .C. (2021). Conc
+000017c0: 6576 6f69 7220 756e 2061 7373 6973 7461  evoir un assista
+000017d0: 6e74 2063 6f6e 7665 7273 6174 696f 6e6e  nt conversationn
+000017e0: 656c 2064 6520 6d61 6e69 c3a8 7265 2069  el de mani..re i
+000017f0: 74c3 a972 6174 6976 6520 6574 2073 656d  t..rative et sem
+00001800: 692d 7375 7065 7276 6973 c3a9 6520 6176  i-supervis..e av
+00001810: 6563 206c 6520 636c 7573 7465 7269 6e67  ec le clustering
+00001820: 2069 6e74 6572 6163 7469 662e 2049 6e20   interactif. In 
+00001830: 4174 656c 6965 7220 2d20 466f 7569 6c6c  Atelier - Fouill
+00001840: 6520 6465 2054 6578 7465 7320 2d20 5465  e de Textes - Te
+00001850: 7874 204d 696e 6520 3230 3231 202d 2045  xt Mine 2021 - E
+00001860: 6e20 636f 6e6a 6f6e 6374 696f 6e20 6176  n conjonction av
+00001870: 6563 2045 4743 2032 3032 312e 20e2 9fa8  ec EGC 2021. ...
+00001880: 6861 6c2d 3033 3133 3330 3630 e29f a92e  hal-03133060....
+00001890: 600a 2020 2020 2d20 496d 706c 656d 656e  `.    - Implemen
+000018a0: 7461 7469 6f6e 3a20 6053 6368 696c 642c  tation: `Schild,
+000018b0: 2045 2e20 2832 3032 3129 2e20 636f 676e   E. (2021). cogn
+000018c0: 6974 6976 6566 6163 746f 7279 2f69 6e74  itivefactory/int
+000018d0: 6572 6163 7469 7665 2d63 6c75 7374 6572  eractive-cluster
+000018e0: 696e 672e 205a 656e 6f64 6f2e 2068 7474  ing. Zenodo. htt
+000018f0: 7073 3a2f 2f64 6f69 2e6f 7267 2f31 302e  ps://doi.org/10.
+00001900: 3532 3831 2f7a 656e 6f64 6f2e 3437 3735  5281/zenodo.4775
+00001910: 3235 312e 600a 0a2d 202a 2a57 6562 2061  251.`..- **Web a
+00001920: 7070 6c69 6361 7469 6f6e 2a2a 3a0a 2020  pplication**:.  
+00001930: 2020 2d20 5f46 6173 7441 5049 5f3a 2060    - _FastAPI_: `
+00001940: 6874 7470 733a 2f2f 6661 7374 6170 692e  https://fastapi.
+00001950: 7469 616e 676f 6c6f 2e63 6f6d 2f60 0a0a  tiangolo.com/`..
+00001960: 0a23 2320 3c61 206e 616d 653d 2248 6f77  .## <a name="How
+00001970: 2074 6f20 6369 7465 223e 3c2f 613e 2048   to cite"></a> H
+00001980: 6f77 2074 6f20 6369 7465 0a0a 6053 6368  ow to cite..`Sch
+00001990: 696c 642c 2045 2e20 2832 3032 3129 2e20  ild, E. (2021). 
+000019a0: 636f 676e 6974 6976 6566 6163 746f 7279  cognitivefactory
+000019b0: 2f69 6e74 6572 6163 7469 7665 2d63 6c75  /interactive-clu
+000019c0: 7374 6572 696e 672d 6775 692e 205a 656e  stering-gui. Zen
+000019d0: 6f64 6f2e 2068 7474 7073 3a2f 2f64 6f69  odo. https://doi
+000019e0: 2e6f 7267 2f31 302e 3532 3831 2f7a 656e  .org/10.5281/zen
+000019f0: 6f64 6f2e 3437 3735 3237 302e 600a       odo.4775270.`.
```

### Comparing `cognitivefactory-interactive-clustering-gui-0.4.0/src/cognitivefactory/interactive_clustering_gui/__main__.py` & `cognitivefactory-interactive-clustering-gui-0.4.1/src/cognitivefactory/interactive_clustering_gui/__main__.py`

 * *Files identical despite different names*

### Comparing `cognitivefactory-interactive-clustering-gui-0.4.0/src/cognitivefactory/interactive_clustering_gui/app.py` & `cognitivefactory-interactive-clustering-gui-0.4.1/src/cognitivefactory/interactive_clustering_gui/app.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 * Licence:      CeCILL-C License v1.0 (https://cecill.info/licences.fr.html)
 """
 
 # ==============================================================================
 # IMPORT PYTHON DEPENDENCIES
 # ==============================================================================
 
+import html
 import json
 import os
 import pathlib
 import shutil
 from datetime import datetime
 from typing import Any, Callable, Dict, List, Optional, Tuple
 
@@ -286,14 +287,15 @@
     return Response(status_code=status.HTTP_200_OK)
 
 
 # ==============================================================================
 # DEFINE ROUTES FOR HOME AND DOCUMENTATION
 # ==============================================================================
 
+
 ###
 ### ROUTE: Get HTML welcome page.
 ###
 @app.get(
     "/",
     tags=["Home and Documentation"],
     response_class=Response,
@@ -610,15 +612,14 @@
 )
 async def get_metadata(
     project_id: str = Path(
         ...,
         description="The ID of the project.",
     ),
 ) -> Dict[str, Any]:
-
     """
     Get metadata.
 
     Args:
         project_id (str): The ID of the project.
 
     Raises:
@@ -635,15 +636,14 @@
             detail="The project with id '{project_id_str}' doesn't exist.".format(
                 project_id_str=str(project_id),
             ),
         )
 
     # Load the project metadata.
     with open(DATA_DIRECTORY / project_id / "metadata.json", "r") as metadata_fileobject:
-
         # Return the project metadata.
         return {
             "project_id": project_id,
             "metadata": json.load(metadata_fileobject),
         }
 
 
@@ -791,15 +791,14 @@
     background_tasks.add_task(
         func=clear_after_import_project,
     )
 
     # Try to open archive file.
     try:
         with zipfile.ZipFile(import_archive_path, "r") as import_archive_file:
-
             ###
             ### Check archive content.
             ###
             missing_files: List[str] = [
                 needed_file
                 for needed_file in (
                     "metadata.json",
@@ -1095,14 +1094,15 @@
         )
 
 
 # ==============================================================================
 # DEFINE ROUTES FOR STATUS
 # ==============================================================================
 
+
 ###
 ### ROUTE: Get status.
 ###
 @app.get(
     "/api/projects/{project_id}/status",
     tags=["Status"],
     status_code=status.HTTP_200_OK,
@@ -1133,15 +1133,14 @@
             detail="The project with id '{project_id_str}' doesn't exist.".format(
                 project_id_str=str(project_id),
             ),
         )
 
     # Load status file.
     with open(DATA_DIRECTORY / project_id / "status.json", "r") as status_fileobject:
-
         project_status: Dict[str, Any] = json.load(status_fileobject)
         project_status["state_details"] = get_ICGUIStates_details(state=project_status["state"])
 
         # Return the requested status.
         return {"project_id": project_id, "status": project_status}
 
 
@@ -1180,15 +1179,14 @@
             detail="The project with id '{project_id_str}' doesn't exist.".format(
                 project_id_str=str(project_id),
             ),
         )
 
     # Lock status file in order to check project status for this step.
     with FileLock(str(DATA_DIRECTORY / project_id / "status.json.lock")):
-
         ###
         ### Load needed data.
         ###
 
         # Load status file.
         with open(DATA_DIRECTORY / project_id / "status.json", "r") as status_fileobject_r:
             project_status: Dict[str, Any] = json.load(status_fileobject_r)
@@ -1351,22 +1349,21 @@
         if sorted_by == TextsSortOptions.ALPHABETICAL:
             return text_to_sort[1]["text_preprocessed"]
         # By deletion status.
         #### if sorted_by == TextsSortOptions.IS_DELETED:
         return text_to_sort[1]["is_deleted"]
 
     # Sorted the texts to return.
-    sorted_texts: Dict[str, Any] = {
-        sorted_text_id: sorted_text
-        for sorted_text_id, sorted_text in sorted(
+    sorted_texts: Dict[str, Any] = dict(
+        sorted(
             texts.items(),
             key=get_value_for_texts_sorting,
             reverse=sorted_reverse,
         )
-    }
+    )
 
     # Return the requested texts.
     return {
         "project_id": project_id,
         "texts": sorted_texts,
         # Get the request parameters.
         "parameters": {
@@ -1418,15 +1415,14 @@
             detail="The project with id '{project_id_str}' doesn't exist.".format(
                 project_id_str=str(project_id),
             ),
         )
 
     # Lock status file in order to check project status for this step.
     with FileLock(str(DATA_DIRECTORY / project_id / "status.json.lock")):
-
         ###
         ### Load needed data.
         ###
 
         # Load status file.
         with open(DATA_DIRECTORY / project_id / "status.json", "r") as status_fileobject:
             project_status: Dict[str, Any] = json.load(status_fileobject)
@@ -1480,15 +1476,14 @@
         ####    project_status["state"] = ICGUIStates.ANNOTATION_WITH_OUTDATED_MODELIZATION_WITH_CONFLICTS
 
         # Update texts by deleting the text.
         texts[text_id]["is_deleted"] = True
 
         # Update constraints by hidding those associated with the deleted text.
         for constraint_id, constraint_value in constraints.items():
-
             data_id1: str = constraint_value["data"]["id_1"]
             data_id2: str = constraint_value["data"]["id_2"]
 
             if text_id in {
                 data_id1,
                 data_id2,
             }:
@@ -1562,15 +1557,14 @@
             detail="The project with id '{project_id_str}' doesn't exist.".format(
                 project_id_str=str(project_id),
             ),
         )
 
     # Lock status file in order to check project status for this step.
     with FileLock(str(DATA_DIRECTORY / project_id / "status.json.lock")):
-
         ###
         ### Load needed data.
         ###
 
         # Load status file.
         with open(DATA_DIRECTORY / project_id / "status.json", "r") as status_fileobject:
             project_status: Dict[str, Any] = json.load(status_fileobject)
@@ -1624,20 +1618,18 @@
         ####    project_status["state"] = ICGUIStates.ANNOTATION_WITH_OUTDATED_MODELIZATION_WITH_CONFLICTS
 
         # Update texts by undeleting the text.
         texts[text_id]["is_deleted"] = False
 
         # Update constraints by unhidding those associated with the undeleted text.
         for constraint_id, constraint_value in constraints.items():
-
             data_id1: str = constraint_value["data"]["id_1"]
             data_id2: str = constraint_value["data"]["id_2"]
 
             if text_id in {data_id1, data_id2}:
-
                 constraints[constraint_id]["is_hidden"] = (
                     texts[data_id1]["is_deleted"] is True or texts[data_id2]["is_deleted"] is True
                 )
 
         ###
         ### Store updated data.
         ###
@@ -1713,15 +1705,14 @@
             detail="The project with id '{project_id_str}' doesn't exist.".format(
                 project_id_str=str(project_id),
             ),
         )
 
     # Lock status file in order to check project status for this step.
     with FileLock(str(DATA_DIRECTORY / project_id / "status.json.lock")):
-
         ###
         ### Load needed data.
         ###
 
         # Load status file.
         with open(DATA_DIRECTORY / project_id / "status.json", "r") as status_fileobject:
             project_status: Dict[str, Any] = json.load(status_fileobject)
@@ -1855,16 +1846,16 @@
                 # Get the project status (iteration, step name and status, modelization state and conflict).
                 "status": (await get_status(project_id=project_id))["status"],
                 # Get the project texts.
                 "texts": (
                     await get_texts(
                         project_id=project_id,
                         without_deleted_texts=False,
-                        sorted_by=sorted_by,
-                        sorted_reverse=sorted_reverse,
+                        sorted_by=TextsSortOptions.ID,
+                        sorted_reverse=False,
                     )
                 )["texts"],
                 # Get the project constraints.
                 "constraints": (
                     await get_constraints(
                         project_id=project_id,
                         without_hidden_constraints=True,
@@ -1994,37 +1985,36 @@
             return (
                 constraint_to_sort[1]["constraint_type"] is None,
                 constraint_to_sort[1]["constraint_type"] == "CANNOT_LINK",
                 constraint_to_sort[1]["constraint_type"] == "MUST_LINK",
             )
         # By date of update.
         if sorted_by == ConstraintsSortOptions.DATE_OF_UPDATE:
-            return constraint_to_sort[1]["date_of_update"]
+            return constraint_to_sort[1]["date_of_update"] if constraint_to_sort[1]["date_of_update"] is not None else 0
         # By iteration of sampling.
         if sorted_by == ConstraintsSortOptions.ITERATION_OF_SAMPLING:
             return constraint_to_sort[1]["iteration_of_sampling"]
         # To annotation.
         if sorted_by == ConstraintsSortOptions.TO_ANNOTATE:
             return constraint_to_sort[1]["to_annotate"] is False
         # To review.
         if sorted_by == ConstraintsSortOptions.TO_REVIEW:
             return constraint_to_sort[1]["to_review"] is False
         # To fix conflict.
         #### if sorted_by == ConstraintsSortOptions.TO_FIX_CONFLICT:
         return constraint_to_sort[1]["to_fix_conflict"] is False
 
     # Sorted the constraints to return.
-    sorted_constraints: Dict[str, Any] = {
-        sorted_constraint_id: sorted_constraint
-        for sorted_constraint_id, sorted_constraint in sorted(
+    sorted_constraints: Dict[str, Any] = dict(
+        sorted(
             constraints.items(),
             key=get_value_for_constraints_sorting,
             reverse=sorted_reverse,
         )
-    }
+    )
 
     # Return the requested constraints.
     return {
         "project_id": project_id,
         "constraints": sorted_constraints,
         # Get the request parameters.
         "parameters": {
@@ -2081,15 +2071,14 @@
             detail="The project with id '{project_id_str}' doesn't exist.".format(
                 project_id_str=str(project_id),
             ),
         )
 
     # Lock status file in order to check project status for this step.
     with FileLock(str(DATA_DIRECTORY / project_id / "status.json.lock")):
-
         ###
         ### Load needed data.
         ###
 
         # Load status file.
         with open(DATA_DIRECTORY / project_id / "status.json", "r") as status_fileobject:
             project_status: Dict[str, Any] = json.load(status_fileobject)
@@ -2217,15 +2206,14 @@
             detail="The project with id '{project_id_str}' doesn't exist.".format(
                 project_id_str=str(project_id),
             ),
         )
 
     # Lock status file in order to check project status for this step.
     with FileLock(str(DATA_DIRECTORY / project_id / "status.json.lock")):
-
         ###
         ### Load needed data.
         ###
 
         # Load constraints file.
         with open(DATA_DIRECTORY / project_id / "constraints.json", "r") as constraints_fileobject_r:
             constraints: Dict[str, Any] = json.load(constraints_fileobject_r)
@@ -2318,15 +2306,14 @@
             detail="The project with id '{project_id_str}' doesn't exist.".format(
                 project_id_str=str(project_id),
             ),
         )
 
     # Lock status file in order to check project status for this step.
     with FileLock(str(DATA_DIRECTORY / project_id / "status.json.lock")):
-
         ###
         ### Load needed data.
         ###
 
         # Load constraints file.
         with open(DATA_DIRECTORY / project_id / "constraints.json", "r") as constraints_fileobject_r:
             constraints: Dict[str, Any] = json.load(constraints_fileobject_r)
@@ -2407,15 +2394,14 @@
             detail="The project with id '{project_id_str}' doesn't exist.".format(
                 project_id_str=str(project_id),
             ),
         )
 
     # Lock status file in order to check project status for this step.
     with FileLock(str(DATA_DIRECTORY / project_id / "status.json.lock")):
-
         # Load status file.
         with open(DATA_DIRECTORY / project_id / "status.json", "r") as status_fileobject:
             project_status: Dict[str, Any] = json.load(status_fileobject)
 
         # Check status.
         if project_status["state"] != ICGUIStates.ANNOTATION_WITH_UPTODATE_MODELIZATION:
             raise HTTPException(
@@ -2594,14 +2580,28 @@
                     await get_texts(
                         project_id=project_id,
                         without_deleted_texts=False,
                         sorted_by=TextsSortOptions.ID,
                         sorted_reverse=False,
                     )
                 )["texts"],
+                "texts_html_escaped": {  # TODO: Escape HTML for javascript
+                    text_id: {  # Force HTML escape.
+                        key: (html.escape(value) if key in {"text_original", "text", "text_preprocessed"} else value)
+                        for key, value in text_value.items()
+                    }
+                    for text_id, text_value in (
+                        await get_texts(
+                            project_id=project_id,
+                            without_deleted_texts=False,
+                            sorted_by=TextsSortOptions.ID,
+                            sorted_reverse=False,
+                        )
+                    )["texts"].items()
+                },
                 # Get the project constraints.
                 "constraints": (
                     await get_constraints(
                         project_id=project_id,
                         without_hidden_constraints=False,
                         sorted_by=ConstraintsSortOptions.ITERATION_OF_SAMPLING,
                         sorted_reverse=False,
@@ -2631,14 +2631,15 @@
         )
 
 
 # ==============================================================================
 # DEFINE ROUTES FOR SETTINGS
 # ==============================================================================
 
+
 ###
 ### ROUTE: Get settings.
 ###
 @app.get(
     "/api/projects/{project_id}/settings",
     tags=["Settings"],
     status_code=status.HTTP_200_OK,
@@ -2787,15 +2788,14 @@
             detail="The project with id '{project_id_str}' doesn't exist.".format(
                 project_id_str=str(project_id),
             ),
         )
 
     # Lock status file in order to check project status for this step.
     with FileLock(str(DATA_DIRECTORY / project_id / "status.json.lock")):
-
         ###
         ### Load needed data.
         ###
 
         # Load status file.
         with open(DATA_DIRECTORY / project_id / "status.json", "r") as status_fileobject_r:
             project_status: Dict[str, Any] = json.load(status_fileobject_r)
@@ -3086,15 +3086,14 @@
             detail="The project with id '{project_id_str}' doesn't exist.".format(
                 project_id_str=str(project_id),
             ),
         )
 
     # Load the modelization inference results.
     with open(DATA_DIRECTORY / project_id / "modelization.json", "r") as modelization_fileobject:
-
         # Return the project modelization inference.
         return {
             "project_id": project_id,
             "modelization": json.load(modelization_fileobject),
         }
 
 
@@ -3217,15 +3216,14 @@
             detail="The project with id '{project_id_str}' doesn't exist.".format(
                 project_id_str=str(project_id),
             ),
         )
 
     # Lock status file in order to check project status for this step.
     with FileLock(str(DATA_DIRECTORY / project_id / "status.json.lock")):
-
         ###
         ### Load needed data.
         ###
 
         # Load status file.
         with open(DATA_DIRECTORY / project_id / "status.json", "r") as status_fileobject:
             project_status: Dict[str, Any] = json.load(status_fileobject)
@@ -3412,15 +3410,14 @@
                 project_id_str=str(project_id),
                 iteration_id_str=str(iteration_id),
             ),
         )
 
     # Load the sampling results.
     with open(DATA_DIRECTORY / project_id / "sampling.json", "r") as sampling_fileobject:
-
         # Return the project sampling.
         return {
             "project_id": project_id,
             "iteration_id": iteration_id,
             "sampling": json.load(sampling_fileobject)[str(iteration_id)],
         }
 
@@ -3462,15 +3459,14 @@
             detail="The project with id '{project_id_str}' doesn't exist.".format(
                 project_id_str=str(project_id),
             ),
         )
 
     # Lock status file in order to check project status for this step.
     with FileLock(str(DATA_DIRECTORY / project_id / "status.json.lock")):
-
         # Load status file.
         with open(DATA_DIRECTORY / project_id / "status.json", "r") as status_fileobject:
             project_status: Dict[str, Any] = json.load(status_fileobject)
 
         # Check status.
         if project_status["state"] != ICGUIStates.SAMPLING_TODO:
             raise HTTPException(
@@ -3664,15 +3660,14 @@
             detail="The project with id '{project_id_str}' doesn't exist.".format(
                 project_id_str=str(project_id),
             ),
         )
 
     # Lock status file in order to check project status for this step.
     with FileLock(str(DATA_DIRECTORY / project_id / "status.json.lock")):
-
         ###
         ### Load needed data.
         ###
 
         # Load status file.
         with open(DATA_DIRECTORY / project_id / "status.json", "r") as status_fileobject:
             project_status: Dict[str, Any] = json.load(status_fileobject)
```

### Comparing `cognitivefactory-interactive-clustering-gui-0.4.0/src/cognitivefactory/interactive_clustering_gui/backgroundtasks.py` & `cognitivefactory-interactive-clustering-gui-0.4.1/src/cognitivefactory/interactive_clustering_gui/backgroundtasks.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,22 +12,17 @@
 # ==============================================================================
 # IMPORT PYTHON DEPENDENCIES
 # ==============================================================================
 
 import json
 import os
 import pathlib
-import sys
+import pickle  # noqa: S403
 from typing import Any, Dict, List, Optional, Tuple
 
-if sys.version_info.minor < 8:  # pragma: nocover
-    import pickle5 as pickle  # noqa: S403
-else:  # pragma: nocover
-    import pickle  # type: ignore # noqa: S403 WPS440
-
 from filelock import FileLock
 from numpy import ndarray
 from scipy.sparse import csr_matrix, vstack
 from sklearn.manifold import TSNE
 
 from cognitivefactory.interactive_clustering.clustering.abstract import AbstractConstrainedClustering
 from cognitivefactory.interactive_clustering.clustering.factory import clustering_factory
@@ -113,14 +108,15 @@
         )
 
 
 # ==============================================================================
 # DEFINE BACKGROUND TASKS FOR MODELIZATION UPDATE
 # ==============================================================================
 
+
 ###
 ### BACKGROUND TASK: Run modelization update task.
 ###
 def run_modelization_update_task(
     project_id: str,
 ) -> None:
     """
@@ -138,15 +134,14 @@
 
     # Check project id : Case of unknown.
     if project_id not in get_projects():
         return
 
     # Lock status file in order to check project status for this step.
     with FileLock(str(DATA_DIRECTORY / project_id / "status.json.lock")):
-
         ###
         ### Load needed data.
         ###
 
         # Load status file.
         with open(DATA_DIRECTORY / project_id / "status.json", "r") as status_fileobject_r:
             project_status: Dict[str, Any] = json.load(status_fileobject_r)
@@ -299,14 +294,15 @@
 
     # Reduce vectors to 2 dimensions with TSNE.
     vectors_2D: ndarray = TSNE(
         n_components=2,
         # learning_rate="auto",  # Error on "scikit-learn==0.24.1" !
         init="random",
         random_state=settings[str(iteration_id)]["vectorization"]["random_seed"],
+        perplexity=min(30.0, vectors_ND.shape[0] - 1),  # TSNE requirement.
     ).fit_transform(vectors_ND)
 
     # Store 2D vectors.
     with open(DATA_DIRECTORY / project_id / "vectors_2D.json", "w") as vectors_2D_fileobject:
         json.dump(
             {
                 text_id_with_2D: {
@@ -331,14 +327,15 @@
 
     # Reduce vectors to 3 dimensions with TSNE.
     vectors_3D: ndarray = TSNE(
         n_components=3,
         # learning_rate="auto",  # Error on "scikit-learn==0.24.1" !
         init="random",
         random_state=settings[str(iteration_id)]["vectorization"]["random_seed"],
+        perplexity=min(30.0, vectors_ND.shape[0] - 1),  # TSNE requirement.
     ).fit_transform(vectors_ND)
 
     # Store 3D vectors.
     with open(DATA_DIRECTORY / project_id / "vectors_3D.json", "w") as vectors_3D_fileobject:
         json.dump(
             {
                 text_id_with_3D: {
@@ -373,37 +370,34 @@
 
     # First, reset `to_fix_conflict` status of all constraints.
     for constraint_id in constraints.keys():
         constraints[constraint_id]["to_fix_conflict"] = False
 
     # Then, update constraints manager with "CANNOT_LINK" constraints.
     for _, constraint_CL in constraints.items():
-
         if constraint_CL["constraint_type"] == "CANNOT_LINK" and constraint_CL["is_hidden"] is False:
             new_constraints_manager.add_constraint(
                 data_ID1=constraint_CL["data"]["id_1"],
                 data_ID2=constraint_CL["data"]["id_2"],
                 constraint_type="CANNOT_LINK",
             )  # No conflict can append, at this step the constraints manager handle only constraints of same type.
 
     # Initialize conflicts counter.
     number_of_conflicts: int = 0
 
     # Finaly, update constraints manager with "MUST_LINK" constraints.
     for constraint_ML_id, constraint_ML in constraints.items():
-
         if constraint_ML["constraint_type"] == "MUST_LINK" and constraint_ML["is_hidden"] is False:
             try:
                 new_constraints_manager.add_constraint(
                     data_ID1=constraint_ML["data"]["id_1"],
                     data_ID2=constraint_ML["data"]["id_2"],
                     constraint_type="MUST_LINK",
                 )  # Conflicts can append.
             except ValueError:
-
                 # Update conflicts status.
                 constraints[constraint_ML_id]["to_fix_conflict"] = True
                 number_of_conflicts += 1
 
     # Store new constraints manager.
     with open(DATA_DIRECTORY / project_id / "constraints_manager.pkl", "wb") as constraints_manager_fileobject:
         pickle.dump(
@@ -496,14 +490,15 @@
         )
 
 
 # ==============================================================================
 # DEFINE BACKGROUND TASKS FOR CONSTRAINTS SAMPLING
 # ==============================================================================
 
+
 ###
 ### BACKGROUND TASK: Run constraints sampling task.
 ###
 def run_constraints_sampling_task(
     project_id: str,
 ) -> None:
     """
@@ -520,15 +515,14 @@
 
     # Check project id : Case of unknown.
     if project_id not in get_projects():
         return
 
     # Lock status file in order to check project iteration and project status for this step.
     with FileLock(str(DATA_DIRECTORY / project_id / "status.json.lock")):
-
         # Load status file.
         with open(DATA_DIRECTORY / project_id / "status.json", "r") as status_fileobject_r:
             project_status: Dict[str, Any] = json.load(status_fileobject_r)
 
         # Check project status.
         if project_status["state"] != ICGUIStates.SAMPLING_PENDING:
             return
@@ -617,19 +611,15 @@
             project_id=project_id,
             task_progression=50,
             task_detail="Initialize constraints sampler.",
         )
 
     # Initialize constraints sampler.
     kwargs_sampling_init: Dict[str, Any] = (
-        {
-            key: value
-            for key, value in settings[str(iteration_id)]["sampling"]["init_kargs"].items()
-            if value is not None
-        }
+        settings[str(iteration_id)]["sampling"]["init_kargs"]
         if (settings[str(iteration_id)]["sampling"]["init_kargs"] is not None)
         else {}
     )
     sampler: AbstractConstraintsSampling = (
         ClustersBasedConstraintsSampling(**kwargs_sampling_init)
         if (settings[str(iteration_id)]["sampling"]["algorithm"] == "custom")
         else sampling_factory(
@@ -699,16 +689,15 @@
     with open(DATA_DIRECTORY / project_id / "constraints.json", "r") as constraints_fileobject_r:
         constraints: Dict[str, Dict[str, Any]] = json.load(constraints_fileobject_r)
 
     # Initialize sampling result for this iteration.
     sampling_results[str(iteration_id)] = []
 
     # For all sampling to annotate...
-    for (data_ID1, data_ID2) in sampling_result:
-
+    for data_ID1, data_ID2 in sampling_result:
         # Define sampling id.
         constraint_id: str = "({data_ID1_str},{data_ID2_str})".format(
             data_ID1_str=data_ID1,
             data_ID2_str=data_ID2,
         )
 
         # Add sampling id.
@@ -763,14 +752,15 @@
         )
 
 
 # ==============================================================================
 # DEFINE BACKGROUND TASKS FOR CONSTRAINED CLUSTERING
 # ==============================================================================
 
+
 ###
 ### BACKGROUND TASK: Run constraints clustering task.
 ###
 def run_constrained_clustering_task(
     project_id: str,
 ) -> None:
     """
@@ -787,15 +777,14 @@
 
     # Check project id : Case of unknown.
     if project_id not in get_projects():
         return
 
     # Lock status file in order to check project status for this step.
     with FileLock(str(DATA_DIRECTORY / project_id / "status.json.lock")):
-
         # Load status file.
         with open(DATA_DIRECTORY / project_id / "status.json", "r") as status_fileobject_r:
             project_status: Dict[str, Any] = json.load(status_fileobject_r)
 
         # Check project status.
         if project_status["state"] != ICGUIStates.CLUSTERING_PENDING:
             return
@@ -865,19 +854,15 @@
             project_id=project_id,
             task_progression=40,
             task_detail="Initialize clustering model.",
         )
 
     # Initialize clustering model.
     kwargs_clustering_init: Dict[str, Any] = (
-        {
-            key: value
-            for key, value in settings[str(iteration_id)]["clustering"]["init_kargs"].items()
-            if value is not None
-        }
+        settings[str(iteration_id)]["clustering"]["init_kargs"]
         if (settings[str(iteration_id)]["clustering"]["init_kargs"] is not None)
         else {}
     )
     clustering_model: AbstractConstrainedClustering = clustering_factory(
         algorithm=settings[str(iteration_id)]["clustering"]["algorithm"],
         random_seed=settings[str(iteration_id)]["clustering"]["random_seed"],
         **kwargs_clustering_init,
```

### Comparing `cognitivefactory-interactive-clustering-gui-0.4.0/src/cognitivefactory/interactive_clustering_gui/cli.py` & `cognitivefactory-interactive-clustering-gui-0.4.1/src/cognitivefactory/interactive_clustering_gui/cli.py`

 * *Files identical despite different names*

### Comparing `cognitivefactory-interactive-clustering-gui-0.4.0/src/cognitivefactory/interactive_clustering_gui/css/new_styles.css` & `cognitivefactory-interactive-clustering-gui-0.4.1/src/cognitivefactory/interactive_clustering_gui/css/new_styles.css`

 * *Files identical despite different names*

### Comparing `cognitivefactory-interactive-clustering-gui-0.4.0/src/cognitivefactory/interactive_clustering_gui/css/styles.css` & `cognitivefactory-interactive-clustering-gui-0.4.1/src/cognitivefactory/interactive_clustering_gui/css/styles.css`

 * *Files identical despite different names*

### Comparing `cognitivefactory-interactive-clustering-gui-0.4.0/src/cognitivefactory/interactive_clustering_gui/html/_base.html` & `cognitivefactory-interactive-clustering-gui-0.4.1/src/cognitivefactory/interactive_clustering_gui/html/_base.html`

 * *Files 10% similar despite different names*

```diff
@@ -14,19 +14,22 @@
 		<meta charset="UTF-8">
 		<meta name="viewport" content="width=device-width, initial-scale=1.0">
 		
 		<!-- Page styles -->
 		<link rel="stylesheet" href="/css/styles.css">
 		<link rel="stylesheet" href="https://fonts.googleapis.com/css2?family=Roboto&display=swap">
 		<link rel="stylesheet" href="https://fonts.googleapis.com/icon?family=Material+Icons"> <!-- Content: https://fonts.google.com/icons?selected=Material+Icons -->
+		<link rel="stylesheet" href="https://unpkg.com/material-components-web@latest/dist/material-components-web.min.css">
 		<link rel="stylesheet" href="https://use.fontawesome.com/releases/v5.8.1/css/all.css" integrity="sha384-50oBUHEmvpQ+1lW4y57PTFmhCaXp0ML5d60M1M7uH2+nqUivzIebhndOJK28anvf" crossorigin="anonymous">
 		{% block header_styles %}
 			<!-- Styles of the page -->
 		{% endblock %}
-		
+
+        <!-- Material scripts -->
+        <script src="https://unpkg.com/material-components-web@latest/dist/material-components-web.min.js"></script>
 		<!-- Page scripts -->
 		<script src="/js/collapsing.js"></script>
 		<script src="/js/goto.js"></script>
 		{% block header_javascripts %}
 			<!-- Scripts of the page -->
 		{% endblock %}
     </head>
```

#### html2text {}

```diff
@@ -1,15 +1,17 @@
 
 
 
 
 
 
 
+
  {% block header_styles %}  {% endblock %}
+
  {% block header_javascripts %}  {% endblock %}
  Interactive Clustering Graphical User Interface
    {% if (projects is defined) or (metadata is defined) %}  arrow_forward_ios
 folder  {% endif %} {% if metadata is defined %}  arrow_forward_ios   home
 {{metadata.project_name}}
 {% endif %}  email   help
 {% block content %} << Insert page content here. >> {% endblock %}
```

### Comparing `cognitivefactory-interactive-clustering-gui-0.4.0/src/cognitivefactory/interactive_clustering_gui/html/analytics.html` & `cognitivefactory-interactive-clustering-gui-0.4.1/src/cognitivefactory/interactive_clustering_gui/html/analytics.html`

 * *Files identical despite different names*

### Comparing `cognitivefactory-interactive-clustering-gui-0.4.0/src/cognitivefactory/interactive_clustering_gui/html/constraint_annotation.html` & `cognitivefactory-interactive-clustering-gui-0.4.1/src/cognitivefactory/interactive_clustering_gui/html/constraint_annotation.html`

 * *Files 1% similar despite different names*

```diff
@@ -308,15 +308,15 @@
 
 							</div>
 							<script>
 								// Get needed data.
 								var dataToPlot = {
 									"projectID": '{{ project_id }}',
 									"constraintID": '{{ constraint_id }}',
-									"texts": JSON.parse('{{ texts | tojson }}'),  // TODO: Read constraint from jinja variable.
+									"texts": JSON.parse('{{ texts_html_escaped | tojson }}'),  // TODO: Read constraint from jinja variable.
 									"constraints": JSON.parse('{{ constraints | tojson }}'),  // TODO: Read constraint from jinja variable.
 									"modelization": JSON.parse('{{ modelization | tojson }}'),  // TODO: Read constraint from jinja variable.
 								}
 
 								// Initialize local constraints graph.
 								plotLocalConstraintsGraph({
 									projectID: dataToPlot["projectID"],
```

### Comparing `cognitivefactory-interactive-clustering-gui-0.4.0/src/cognitivefactory/interactive_clustering_gui/html/constraints.html` & `cognitivefactory-interactive-clustering-gui-0.4.1/src/cognitivefactory/interactive_clustering_gui/html/constraints.html`

 * *Files 0% similar despite different names*

```diff
@@ -338,15 +338,15 @@
 							<td class="column center" title="Constraint ID: {{ constraint_id }}">
 								<select 
 									required
 									{% if modification_disabled %}disabled{% endif %}
 									class="{% if constraint.constraint_type == 'MUST_LINK' %}background_must_link{% elif constraint.constraint_type == 'CANNOT_LINK' %}background_cannot_link{% else %}background_blank{% endif %}"
 									id="{{ constraint_id }}.select"
 									style="font-size: 1em; width: 100%;"
-									onchange="this.disabled=true; this.classList=this.options[this.selectedIndex].classList; updateConstraint({projectID:'{{project_id}}', constraintID:'{{constraint_id}}', constraintType:this.value, reloadOption:true});">
+									onchange="this.classList=this.options[this.selectedIndex].classList; updateConstraint({projectID:'{{project_id}}', constraintID:'{{constraint_id}}', constraintType:this.value, reloadOption:false});">
 									<option
 										value=""
 										{% if constraint.constraint_type is none %}selected{% endif %}
 										class="background_blank">
 										SKIP
 									</option>
 									<option
```

#### html2text {}

```diff
@@ -69,43 +69,37 @@
 update
 % if parameters.sorted_by=="to_annotate" %}selected{% endif %}> to annotate
 % if parameters.sorted_by=="to_review" %}selected{% endif %}> to review
 % if parameters.sorted_by=="to_fix_conflict" %}selected{% endif %}> to fix
 conflict
 % if parameters.sorted_reverse==false %}selected{% endif %}> descending
 % if parameters.sorted_reverse==true %}selected{% endif %}> ascending
-Text 1                                                    Constraint                      Text 2                                                    Sampling                         Last                                        To                     To                         To                         Go
-                                                                                                                                                    iteration                        update                                      annotate               review                     fix                        to
-                                                          % if modification_disabled
-                                                          %}disabled{% endif %} class="{%
-                                                          if constraint.constraint_type
-                                                          == 'MUST_LINK'
-                                                          %}background_must_link{% elif
+Text 1                                                    Constraint                            Text 2                                                    Sampling                         Last                                        To                     To                         To                         Go
+                                                                                                                                                          iteration                        update                                      annotate               review                     fix                        to
+                                                          % if modification_disabled %}disabled
+                                                          {% endif %} class="{% if
                                                           constraint.constraint_type ==
+                                                          'MUST_LINK' %}background_must_link{%
+                                                          elif constraint.constraint_type ==
                                                           'CANNOT_LINK'
                                                           %}background_cannot_link{% else
-                                                          %}background_blank{% endif %}"
-                                                          id="{{ constraint_id }}.select"
-                                                          style="font-size: 1em; width:                                                                                                                                                                 % if
-                                                          100%;"                                                                                                                                                                                        constraint.to_review==true
-                                                          onchange="this.disabled=true;                                                                                              {% if constraint.date_of_update is none %}                         %}checked{% endif %}       {% if                      % if modification_disabled %}disabled
-                                                          this.classList=this.options                                                                                                Never {% else %} {                                                 onchange="reviewConstraint constraint.to_fix_conflict {% endif %} class="material-icons"
-                                                          [this.selectedIndex].classList;                                                           {                                {                                           {% if                  ({projectID:'{             == true %}  priority_high  onclick="goToConstraintsAnnotationPage
-« {{ texts[constraint.data.id_1].text_preprocessed }} » updateConstraint({projectID:'{  « {{ texts[constraint.data.id_2].text_preprocessed }} » {                                constraint.date_of_update|timestamp_to_date constraint.to_annotate {project_id}}',            {% elif                    ({projectID:'{{project_id}}',
-info                                                      {project_id}}', constraintID:'{ info                                                      constraint.iteration_of_sampling }},                                         == true %}             constraintID:'{            constraint.constraint_type constraintID:'{{constraint_id}}'});"
-                                                          {constraint_id}}',                                                                        }}                               at {                                        question_mark  {%      {constraint_id}}',         is not none %}  done  {%   title="Go to a more detailled view of
-                                                          constraintType:this.value,                                                                                                 {                                           endif %}               toReview:this.checked,     else %}  question_mark  {% the constraint {{ constraint_id }}.">
-                                                          reloadOption:true});">                                                                                                     constraint.date_of_update|timestamp_to_hour                        reloadOption:false});"> {% endif %}                   chevron_right
-                                                          % if constraint.constraint_type                                                                                            }}. {% endif %}                                                    if constraint.comment !=
-                                                          is none %}selected{% endif %}                                                                                                                                                                 "" %}  info  {% endif %}
-                                                          class="background_blank"> SKIP
-                                                          % if constraint.constraint_type
-                                                          == "MUST_LINK" %}selected{%
-                                                          endif %}
+                                                          %}background_blank{% endif %}" id="{                                                                                                                                                                % if
+                                                          { constraint_id }}.select"                                                                                                                                                                          constraint.to_review==true
+                                                          style="font-size: 1em; width: 100%;"                                                                                             {% if constraint.date_of_update is none %}                         %}checked{% endif %}       {% if                      % if modification_disabled %}disabled
+                                                          onchange="this.classList=this.options                                                                                            Never {% else %} {                                                 onchange="reviewConstraint constraint.to_fix_conflict {% endif %} class="material-icons"
+                                                          [this.selectedIndex].classList;                                                                 {                                {                                           {% if                  ({projectID:'{             == true %}  priority_high  onclick="goToConstraintsAnnotationPage
+« {{ texts[constraint.data.id_1].text_preprocessed }} » updateConstraint({projectID:'{        « {{ texts[constraint.data.id_2].text_preprocessed }} » {                                constraint.date_of_update|timestamp_to_date constraint.to_annotate {project_id}}',            {% elif                    ({projectID:'{{project_id}}',
+info                                                      {project_id}}', constraintID:'{       info                                                      constraint.iteration_of_sampling }},                                         == true %}             constraintID:'{            constraint.constraint_type constraintID:'{{constraint_id}}'});"
+                                                          {constraint_id}}', constraintType:                                                              }}                               at {                                        question_mark  {%      {constraint_id}}',         is not none %}  done  {%   title="Go to a more detailled view of
+                                                          this.value, reloadOption:false});">                                                                                              {                                           endif %}               toReview:this.checked,     else %}  question_mark  {% the constraint {{ constraint_id }}.">
+                                                          % if constraint.constraint_type is                                                                                               constraint.date_of_update|timestamp_to_hour                        reloadOption:false});"> {% endif %}                   chevron_right
+                                                          none %}selected{% endif %}                                                                                                       }}. {% endif %}                                                    if constraint.comment !=
+                                                          class="background_blank"> SKIP                                                                                                                                                                      "" %}  info  {% endif %}
+                                                          % if constraint.constraint_type ==
+                                                          "MUST_LINK" %}selected{% endif %}
                                                           class="background_must_link">
                                                           MUST_LINK
-                                                          % if constraint.constraint_type
-                                                          == "CANNOT_LINK" %}selected{%
-                                                          endif %}
+                                                          % if constraint.constraint_type ==
+                                                          "CANNOT_LINK" %}selected{% endif %}
                                                           class="background_cannot_link">
                                                           CANNOT_LINK
 {% endblock %}
```

### Comparing `cognitivefactory-interactive-clustering-gui-0.4.0/src/cognitivefactory/interactive_clustering_gui/html/error.html` & `cognitivefactory-interactive-clustering-gui-0.4.1/src/cognitivefactory/interactive_clustering_gui/html/error.html`

 * *Files identical despite different names*

### Comparing `cognitivefactory-interactive-clustering-gui-0.4.0/src/cognitivefactory/interactive_clustering_gui/html/help.html` & `cognitivefactory-interactive-clustering-gui-0.4.1/src/cognitivefactory/interactive_clustering_gui/html/help.html`

 * *Files identical despite different names*

### Comparing `cognitivefactory-interactive-clustering-gui-0.4.0/src/cognitivefactory/interactive_clustering_gui/html/project_home.html` & `cognitivefactory-interactive-clustering-gui-0.4.1/src/cognitivefactory/interactive_clustering_gui/html/project_home.html`

 * *Files identical despite different names*

### Comparing `cognitivefactory-interactive-clustering-gui-0.4.0/src/cognitivefactory/interactive_clustering_gui/html/projects_listing.html` & `cognitivefactory-interactive-clustering-gui-0.4.1/src/cognitivefactory/interactive_clustering_gui/html/projects_listing.html`

 * *Files identical despite different names*

### Comparing `cognitivefactory-interactive-clustering-gui-0.4.0/src/cognitivefactory/interactive_clustering_gui/html/settings.html` & `cognitivefactory-interactive-clustering-gui-0.4.1/src/cognitivefactory/interactive_clustering_gui/html/settings.html`

 * *Files identical despite different names*

### Comparing `cognitivefactory-interactive-clustering-gui-0.4.0/src/cognitivefactory/interactive_clustering_gui/html/texts.html` & `cognitivefactory-interactive-clustering-gui-0.4.1/src/cognitivefactory/interactive_clustering_gui/html/texts.html`

 * *Files 7% similar despite different names*

```diff
@@ -288,15 +288,15 @@
 										onclick="document.getElementById('{{text_id}}.edit').classList.add('hide'); document.getElementById('{{text_id}}.print').classList.remove('hide');">
 										Reset
 									</button>
 									<button
 										class="button_form_submit"
 										id="button_renaming_text_submit"
 										title="Update text renaming."
-										onclick="this.disabled=true; renameText({projectID:'{{project_id}}', textID:'{{text_id}}', newTextValue:document.getElementById('{{ text_id }}.edit.input').value, reloadOption:true});">
+										onclick="renameText({projectID:'{{project_id}}', textID:'{{text_id}}', newTextValue:document.getElementById('{{ text_id }}.edit.input').value, reloadOption:false}); document.getElementById('{{text_id}}.print').getElementsByTagName('i')[0].innerHTML = '&laquo; ' + document.getElementById('{{text_id}}.edit.input').value + ' &raquo;'; document.getElementById('{{text_id}}.edit').classList.add('hide'); document.getElementById('{{text_id}}.print').classList.remove('hide');">
 										Update
 									</button>
 								</form>
 							</td>
 							<td class="column center">
 								<input
 									{% if modification_disabled %}disabled{% endif %}
```

### Comparing `cognitivefactory-interactive-clustering-gui-0.4.0/src/cognitivefactory/interactive_clustering_gui/html/welcome.html` & `cognitivefactory-interactive-clustering-gui-0.4.1/src/cognitivefactory/interactive_clustering_gui/html/welcome.html`

 * *Files identical despite different names*

### Comparing `cognitivefactory-interactive-clustering-gui-0.4.0/src/cognitivefactory/interactive_clustering_gui/js/analytics.js` & `cognitivefactory-interactive-clustering-gui-0.4.1/src/cognitivefactory/interactive_clustering_gui/js/analytics.js`

 * *Files identical despite different names*

### Comparing `cognitivefactory-interactive-clustering-gui-0.4.0/src/cognitivefactory/interactive_clustering_gui/js/annotation.js` & `cognitivefactory-interactive-clustering-gui-0.4.1/src/cognitivefactory/interactive_clustering_gui/js/annotation.js`

 * *Files identical despite different names*

### Comparing `cognitivefactory-interactive-clustering-gui-0.4.0/src/cognitivefactory/interactive_clustering_gui/js/collapsing.js` & `cognitivefactory-interactive-clustering-gui-0.4.1/src/cognitivefactory/interactive_clustering_gui/js/collapsing.js`

 * *Files identical despite different names*

### Comparing `cognitivefactory-interactive-clustering-gui-0.4.0/src/cognitivefactory/interactive_clustering_gui/js/constraints.js` & `cognitivefactory-interactive-clustering-gui-0.4.1/src/cognitivefactory/interactive_clustering_gui/js/constraints.js`

 * *Files identical despite different names*

### Comparing `cognitivefactory-interactive-clustering-gui-0.4.0/src/cognitivefactory/interactive_clustering_gui/js/goto.js` & `cognitivefactory-interactive-clustering-gui-0.4.1/src/cognitivefactory/interactive_clustering_gui/js/goto.js`

 * *Files identical despite different names*

### Comparing `cognitivefactory-interactive-clustering-gui-0.4.0/src/cognitivefactory/interactive_clustering_gui/js/projects.js` & `cognitivefactory-interactive-clustering-gui-0.4.1/src/cognitivefactory/interactive_clustering_gui/js/projects.js`

 * *Files identical despite different names*

### Comparing `cognitivefactory-interactive-clustering-gui-0.4.0/src/cognitivefactory/interactive_clustering_gui/js/projects_listing.js` & `cognitivefactory-interactive-clustering-gui-0.4.1/src/cognitivefactory/interactive_clustering_gui/js/projects_listing.js`

 * *Files identical despite different names*

### Comparing `cognitivefactory-interactive-clustering-gui-0.4.0/src/cognitivefactory/interactive_clustering_gui/js/settings.js` & `cognitivefactory-interactive-clustering-gui-0.4.1/src/cognitivefactory/interactive_clustering_gui/js/settings.js`

 * *Files identical despite different names*

### Comparing `cognitivefactory-interactive-clustering-gui-0.4.0/src/cognitivefactory/interactive_clustering_gui/js/status.js` & `cognitivefactory-interactive-clustering-gui-0.4.1/src/cognitivefactory/interactive_clustering_gui/js/status.js`

 * *Files identical despite different names*

### Comparing `cognitivefactory-interactive-clustering-gui-0.4.0/src/cognitivefactory/interactive_clustering_gui/js/tasks.js` & `cognitivefactory-interactive-clustering-gui-0.4.1/src/cognitivefactory/interactive_clustering_gui/js/tasks.js`

 * *Files identical despite different names*

### Comparing `cognitivefactory-interactive-clustering-gui-0.4.0/src/cognitivefactory/interactive_clustering_gui/models/queries.py` & `cognitivefactory-interactive-clustering-gui-0.4.1/src/cognitivefactory/interactive_clustering_gui/models/queries.py`

 * *Files identical despite different names*

### Comparing `cognitivefactory-interactive-clustering-gui-0.4.0/src/cognitivefactory/interactive_clustering_gui/models/settings.py` & `cognitivefactory-interactive-clustering-gui-0.4.1/src/cognitivefactory/interactive_clustering_gui/models/settings.py`

 * *Files identical despite different names*

### Comparing `cognitivefactory-interactive-clustering-gui-0.4.0/src/cognitivefactory/interactive_clustering_gui/models/states.py` & `cognitivefactory-interactive-clustering-gui-0.4.1/src/cognitivefactory/interactive_clustering_gui/models/states.py`

 * *Files identical despite different names*

### Comparing `cognitivefactory-interactive-clustering-gui-0.4.0/src/cognitivefactory/interactive_clustering_gui/resources/diagrams/example_clustering.png` & `cognitivefactory-interactive-clustering-gui-0.4.1/src/cognitivefactory/interactive_clustering_gui/resources/diagrams/example_clustering.png`

 * *Files identical despite different names*

### Comparing `cognitivefactory-interactive-clustering-gui-0.4.0/src/cognitivefactory/interactive_clustering_gui/resources/diagrams/example_constrained_clustering.png` & `cognitivefactory-interactive-clustering-gui-0.4.1/src/cognitivefactory/interactive_clustering_gui/resources/diagrams/example_constrained_clustering.png`

 * *Files identical despite different names*

### Comparing `cognitivefactory-interactive-clustering-gui-0.4.0/src/cognitivefactory/interactive_clustering_gui/resources/diagrams/example_constraints.png` & `cognitivefactory-interactive-clustering-gui-0.4.1/src/cognitivefactory/interactive_clustering_gui/resources/diagrams/example_constraints.png`

 * *Files identical despite different names*

### Comparing `cognitivefactory-interactive-clustering-gui-0.4.0/src/cognitivefactory/interactive_clustering_gui/resources/diagrams/example_constraints_conflict.png` & `cognitivefactory-interactive-clustering-gui-0.4.1/src/cognitivefactory/interactive_clustering_gui/resources/diagrams/example_constraints_conflict.png`

 * *Files identical despite different names*

### Comparing `cognitivefactory-interactive-clustering-gui-0.4.0/src/cognitivefactory/interactive_clustering_gui/resources/diagrams/example_constraints_inference_cannot_link.png` & `cognitivefactory-interactive-clustering-gui-0.4.1/src/cognitivefactory/interactive_clustering_gui/resources/diagrams/example_constraints_inference_cannot_link.png`

 * *Files identical despite different names*

### Comparing `cognitivefactory-interactive-clustering-gui-0.4.0/src/cognitivefactory/interactive_clustering_gui/resources/diagrams/example_constraints_inference_must_link.png` & `cognitivefactory-interactive-clustering-gui-0.4.1/src/cognitivefactory/interactive_clustering_gui/resources/diagrams/example_constraints_inference_must_link.png`

 * *Files identical despite different names*

### Comparing `cognitivefactory-interactive-clustering-gui-0.4.0/src/cognitivefactory/interactive_clustering_gui/resources/diagrams/example_sampling.png` & `cognitivefactory-interactive-clustering-gui-0.4.1/src/cognitivefactory/interactive_clustering_gui/resources/diagrams/example_sampling.png`

 * *Files identical despite different names*

### Comparing `cognitivefactory-interactive-clustering-gui-0.4.0/src/cognitivefactory/interactive_clustering_gui/resources/diagrams/interactive_clustering.png` & `cognitivefactory-interactive-clustering-gui-0.4.1/src/cognitivefactory/interactive_clustering_gui/resources/diagrams/interactive_clustering.png`

 * *Files identical despite different names*

### Comparing `cognitivefactory-interactive-clustering-gui-0.4.0/src/cognitivefactory/interactive_clustering_gui/resources/logos/github.png` & `cognitivefactory-interactive-clustering-gui-0.4.1/src/cognitivefactory/interactive_clustering_gui/resources/logos/github.png`

 * *Files identical despite different names*

### Comparing `cognitivefactory-interactive-clustering-gui-0.4.0/src/cognitivefactory/interactive_clustering_gui/resources/logos/interactive_clustering_black.png` & `cognitivefactory-interactive-clustering-gui-0.4.1/src/cognitivefactory/interactive_clustering_gui/resources/logos/interactive_clustering_black.png`

 * *Files identical despite different names*

### Comparing `cognitivefactory-interactive-clustering-gui-0.4.0/src/cognitivefactory/interactive_clustering_gui/resources/logos/interactive_clustering_blue.png` & `cognitivefactory-interactive-clustering-gui-0.4.1/src/cognitivefactory/interactive_clustering_gui/resources/logos/interactive_clustering_blue.png`

 * *Files identical despite different names*

### Comparing `cognitivefactory-interactive-clustering-gui-0.4.0/src/cognitivefactory/interactive_clustering_gui/resources/logos/interactive_clustering_gray_1.png` & `cognitivefactory-interactive-clustering-gui-0.4.1/src/cognitivefactory/interactive_clustering_gui/resources/logos/interactive_clustering_gray_1.png`

 * *Files identical despite different names*

### Comparing `cognitivefactory-interactive-clustering-gui-0.4.0/src/cognitivefactory/interactive_clustering_gui/resources/logos/interactive_clustering_gray_2.png` & `cognitivefactory-interactive-clustering-gui-0.4.1/src/cognitivefactory/interactive_clustering_gui/resources/logos/interactive_clustering_gray_2.png`

 * *Files identical despite different names*

### Comparing `cognitivefactory-interactive-clustering-gui-0.4.0/src/cognitivefactory/interactive_clustering_gui/resources/logos/interactive_clustering_pink.png` & `cognitivefactory-interactive-clustering-gui-0.4.1/src/cognitivefactory/interactive_clustering_gui/resources/logos/interactive_clustering_pink.png`

 * *Files identical despite different names*

### Comparing `cognitivefactory-interactive-clustering-gui-0.4.0/src/cognitivefactory/interactive_clustering_gui/resources/logos/interactive_clustering_white.png` & `cognitivefactory-interactive-clustering-gui-0.4.1/src/cognitivefactory/interactive_clustering_gui/resources/logos/interactive_clustering_white.png`

 * *Files identical despite different names*

### Comparing `cognitivefactory-interactive-clustering-gui-0.4.0/tests/conftest.py` & `cognitivefactory-interactive-clustering-gui-0.4.1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/0a_INITIALIZATION_WITHOUT_MODELIZATION/modelization.json` & `cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/0a_INITIALIZATION_WITHOUT_MODELIZATION/modelization.json`

 * *Files identical despite different names*

### Comparing `cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/0a_INITIALIZATION_WITHOUT_MODELIZATION/settings.json` & `cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/0a_INITIALIZATION_WITHOUT_MODELIZATION/settings.json`

 * *Files identical despite different names*

### Comparing `cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/0a_INITIALIZATION_WITHOUT_MODELIZATION/texts.json` & `cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/0a_INITIALIZATION_WITHOUT_MODELIZATION/texts.json`

 * *Files identical despite different names*

### Comparing `cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/0b_INITIALIZATION_WITH_PENDING_MODELIZATION/modelization.json` & `cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/0b_INITIALIZATION_WITH_PENDING_MODELIZATION/modelization.json`

 * *Files identical despite different names*

### Comparing `cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/0b_INITIALIZATION_WITH_PENDING_MODELIZATION/settings.json` & `cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/0b_INITIALIZATION_WITH_PENDING_MODELIZATION/settings.json`

 * *Files identical despite different names*

### Comparing `cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/0b_INITIALIZATION_WITH_PENDING_MODELIZATION/texts.json` & `cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/0b_INITIALIZATION_WITH_PENDING_MODELIZATION/texts.json`

 * *Files identical despite different names*

### Comparing `cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/0c_INITIALIZATION_WITH_WORKING_MODELIZATION/modelization.json` & `cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/0c_INITIALIZATION_WITH_WORKING_MODELIZATION/modelization.json`

 * *Files identical despite different names*

### Comparing `cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/0c_INITIALIZATION_WITH_WORKING_MODELIZATION/settings.json` & `cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/0c_INITIALIZATION_WITH_WORKING_MODELIZATION/settings.json`

 * *Files identical despite different names*

### Comparing `cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/0c_INITIALIZATION_WITH_WORKING_MODELIZATION/texts.json` & `cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/0c_INITIALIZATION_WITH_WORKING_MODELIZATION/texts.json`

 * *Files identical despite different names*

### Comparing `cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/0d_CLUSTERING_TODO/constraints_manager.pkl` & `cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/0d_CLUSTERING_TODO/constraints_manager.pkl`

 * *Files identical despite different names*

### Comparing `cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/0d_CLUSTERING_TODO/modelization.json` & `cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/0d_CLUSTERING_TODO/modelization.json`

 * *Files identical despite different names*

### Comparing `cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/0d_CLUSTERING_TODO/settings.json` & `cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/0d_CLUSTERING_TODO/settings.json`

 * *Files identical despite different names*

### Comparing `cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/0d_CLUSTERING_TODO/texts.json` & `cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/0d_CLUSTERING_TODO/texts.json`

 * *Files identical despite different names*

### Comparing `cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/0d_CLUSTERING_TODO/vectors.pkl` & `cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/0d_CLUSTERING_TODO/vectors.pkl`

 * *Files identical despite different names*

### Comparing `cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/0d_CLUSTERING_TODO/vectors_2D.json` & `cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/0d_CLUSTERING_TODO/vectors_2D.json`

 * *Files identical despite different names*

### Comparing `cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/0d_CLUSTERING_TODO/vectors_3D.json` & `cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/0d_CLUSTERING_TODO/vectors_3D.json`

 * *Files identical despite different names*

### Comparing `cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/0e_CLUSTERING_PENDING/constraints_manager.pkl` & `cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/0e_CLUSTERING_PENDING/constraints_manager.pkl`

 * *Files identical despite different names*

### Comparing `cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/0e_CLUSTERING_PENDING/modelization.json` & `cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/0e_CLUSTERING_PENDING/modelization.json`

 * *Files identical despite different names*

### Comparing `cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/0e_CLUSTERING_PENDING/settings.json` & `cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/0e_CLUSTERING_PENDING/settings.json`

 * *Files identical despite different names*

### Comparing `cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/0e_CLUSTERING_PENDING/texts.json` & `cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/0e_CLUSTERING_PENDING/texts.json`

 * *Files identical despite different names*

### Comparing `cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/0e_CLUSTERING_PENDING/vectors.pkl` & `cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/0e_CLUSTERING_PENDING/vectors.pkl`

 * *Files identical despite different names*

### Comparing `cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/0e_CLUSTERING_PENDING/vectors_2D.json` & `cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/0e_CLUSTERING_PENDING/vectors_2D.json`

 * *Files identical despite different names*

### Comparing `cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/0e_CLUSTERING_PENDING/vectors_3D.json` & `cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/0e_CLUSTERING_PENDING/vectors_3D.json`

 * *Files identical despite different names*

### Comparing `cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/0f_CLUSTERING_WORKING/constraints_manager.pkl` & `cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/0f_CLUSTERING_WORKING/constraints_manager.pkl`

 * *Files identical despite different names*

### Comparing `cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/0f_CLUSTERING_WORKING/modelization.json` & `cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/0f_CLUSTERING_WORKING/modelization.json`

 * *Files identical despite different names*

### Comparing `cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/0f_CLUSTERING_WORKING/settings.json` & `cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/0f_CLUSTERING_WORKING/settings.json`

 * *Files identical despite different names*

### Comparing `cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/0f_CLUSTERING_WORKING/texts.json` & `cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/0f_CLUSTERING_WORKING/texts.json`

 * *Files identical despite different names*

### Comparing `cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/0f_CLUSTERING_WORKING/vectors.pkl` & `cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/0f_CLUSTERING_WORKING/vectors.pkl`

 * *Files identical despite different names*

### Comparing `cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/0f_CLUSTERING_WORKING/vectors_2D.json` & `cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/0f_CLUSTERING_WORKING/vectors_2D.json`

 * *Files identical despite different names*

### Comparing `cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/0f_CLUSTERING_WORKING/vectors_3D.json` & `cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/0f_CLUSTERING_WORKING/vectors_3D.json`

 * *Files identical despite different names*

### Comparing `cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/0g_ITERATION_END/constraints_manager.pkl` & `cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/0g_ITERATION_END/constraints_manager.pkl`

 * *Files identical despite different names*

### Comparing `cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/0g_ITERATION_END/modelization.json` & `cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/0g_ITERATION_END/modelization.json`

 * *Files identical despite different names*

### Comparing `cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/0g_ITERATION_END/settings.json` & `cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/0g_ITERATION_END/settings.json`

 * *Files identical despite different names*

### Comparing `cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/0g_ITERATION_END/texts.json` & `cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/0g_ITERATION_END/texts.json`

 * *Files identical despite different names*

### Comparing `cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/0g_ITERATION_END/vectors.pkl` & `cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/0g_ITERATION_END/vectors.pkl`

 * *Files identical despite different names*

### Comparing `cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/0g_ITERATION_END/vectors_2D.json` & `cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/0g_ITERATION_END/vectors_2D.json`

 * *Files identical despite different names*

### Comparing `cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/0g_ITERATION_END/vectors_3D.json` & `cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/0g_ITERATION_END/vectors_3D.json`

 * *Files identical despite different names*

### Comparing `cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/1a_SAMPLING_TODO/constraints_manager.pkl` & `cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/1a_SAMPLING_TODO/constraints_manager.pkl`

 * *Files identical despite different names*

### Comparing `cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/1a_SAMPLING_TODO/modelization.json` & `cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/1a_SAMPLING_TODO/modelization.json`

 * *Files identical despite different names*

### Comparing `cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/1a_SAMPLING_TODO/settings.json` & `cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/1a_SAMPLING_TODO/settings.json`

 * *Files identical despite different names*

### Comparing `cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/1a_SAMPLING_TODO/texts.json` & `cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/1a_SAMPLING_TODO/texts.json`

 * *Files identical despite different names*

### Comparing `cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/1a_SAMPLING_TODO/vectors.pkl` & `cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/1a_SAMPLING_TODO/vectors.pkl`

 * *Files identical despite different names*

### Comparing `cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/1a_SAMPLING_TODO/vectors_2D.json` & `cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/1a_SAMPLING_TODO/vectors_2D.json`

 * *Files identical despite different names*

### Comparing `cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/1a_SAMPLING_TODO/vectors_3D.json` & `cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/1a_SAMPLING_TODO/vectors_3D.json`

 * *Files identical despite different names*

### Comparing `cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/1b_SAMPLING_PENDING/constraints_manager.pkl` & `cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/1b_SAMPLING_PENDING/constraints_manager.pkl`

 * *Files identical despite different names*

### Comparing `cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/1b_SAMPLING_PENDING/modelization.json` & `cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/1b_SAMPLING_PENDING/modelization.json`

 * *Files identical despite different names*

### Comparing `cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/1b_SAMPLING_PENDING/settings.json` & `cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/1b_SAMPLING_PENDING/settings.json`

 * *Files identical despite different names*

### Comparing `cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/1b_SAMPLING_PENDING/texts.json` & `cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/1b_SAMPLING_PENDING/texts.json`

 * *Files identical despite different names*

### Comparing `cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/1b_SAMPLING_PENDING/vectors.pkl` & `cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/1b_SAMPLING_PENDING/vectors.pkl`

 * *Files identical despite different names*

### Comparing `cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/1b_SAMPLING_PENDING/vectors_2D.json` & `cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/1b_SAMPLING_PENDING/vectors_2D.json`

 * *Files identical despite different names*

### Comparing `cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/1b_SAMPLING_PENDING/vectors_3D.json` & `cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/1b_SAMPLING_PENDING/vectors_3D.json`

 * *Files identical despite different names*

### Comparing `cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/1c_SAMPLING_WORKING/constraints_manager.pkl` & `cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/1c_SAMPLING_WORKING/constraints_manager.pkl`

 * *Files identical despite different names*

### Comparing `cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/1c_SAMPLING_WORKING/modelization.json` & `cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/1c_SAMPLING_WORKING/modelization.json`

 * *Files identical despite different names*

### Comparing `cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/1c_SAMPLING_WORKING/settings.json` & `cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/1c_SAMPLING_WORKING/settings.json`

 * *Files identical despite different names*

### Comparing `cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/1c_SAMPLING_WORKING/texts.json` & `cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/1c_SAMPLING_WORKING/texts.json`

 * *Files identical despite different names*

### Comparing `cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/1c_SAMPLING_WORKING/vectors.pkl` & `cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/1c_SAMPLING_WORKING/vectors.pkl`

 * *Files identical despite different names*

### Comparing `cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/1c_SAMPLING_WORKING/vectors_2D.json` & `cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/1c_SAMPLING_WORKING/vectors_2D.json`

 * *Files identical despite different names*

### Comparing `cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/1c_SAMPLING_WORKING/vectors_3D.json` & `cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/1c_SAMPLING_WORKING/vectors_3D.json`

 * *Files identical despite different names*

### Comparing `cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/1d_ANNOTATION_WITH_UPTODATE_MODELIZATION/constraints.json` & `cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/1d_ANNOTATION_WITH_UPTODATE_MODELIZATION/constraints.json`

 * *Files identical despite different names*

### Comparing `cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/1d_ANNOTATION_WITH_UPTODATE_MODELIZATION/constraints_manager.pkl` & `cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/1d_ANNOTATION_WITH_UPTODATE_MODELIZATION/constraints_manager.pkl`

 * *Files identical despite different names*

### Comparing `cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/1d_ANNOTATION_WITH_UPTODATE_MODELIZATION/modelization.json` & `cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/1d_ANNOTATION_WITH_UPTODATE_MODELIZATION/modelization.json`

 * *Files identical despite different names*

### Comparing `cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/1d_ANNOTATION_WITH_UPTODATE_MODELIZATION/settings.json` & `cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/1d_ANNOTATION_WITH_UPTODATE_MODELIZATION/settings.json`

 * *Files identical despite different names*

### Comparing `cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/1d_ANNOTATION_WITH_UPTODATE_MODELIZATION/texts.json` & `cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/1d_ANNOTATION_WITH_UPTODATE_MODELIZATION/texts.json`

 * *Files identical despite different names*

### Comparing `cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/1d_ANNOTATION_WITH_UPTODATE_MODELIZATION/vectors.pkl` & `cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/1d_ANNOTATION_WITH_UPTODATE_MODELIZATION/vectors.pkl`

 * *Files identical despite different names*

### Comparing `cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/1d_ANNOTATION_WITH_UPTODATE_MODELIZATION/vectors_2D.json` & `cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/1d_ANNOTATION_WITH_UPTODATE_MODELIZATION/vectors_2D.json`

 * *Files identical despite different names*

### Comparing `cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/1d_ANNOTATION_WITH_UPTODATE_MODELIZATION/vectors_3D.json` & `cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/1d_ANNOTATION_WITH_UPTODATE_MODELIZATION/vectors_3D.json`

 * *Files identical despite different names*

### Comparing `cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/1e_ANNOTATION_WITH_OUTDATED_MODELIZATION_WITHOUT_CONFLICTS/constraints.json` & `cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/1e_ANNOTATION_WITH_OUTDATED_MODELIZATION_WITHOUT_CONFLICTS/constraints.json`

 * *Files identical despite different names*

### Comparing `cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/1e_ANNOTATION_WITH_OUTDATED_MODELIZATION_WITHOUT_CONFLICTS/constraints_manager.pkl` & `cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/1e_ANNOTATION_WITH_OUTDATED_MODELIZATION_WITHOUT_CONFLICTS/constraints_manager.pkl`

 * *Files identical despite different names*

### Comparing `cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/1e_ANNOTATION_WITH_OUTDATED_MODELIZATION_WITHOUT_CONFLICTS/modelization.json` & `cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/1e_ANNOTATION_WITH_OUTDATED_MODELIZATION_WITHOUT_CONFLICTS/modelization.json`

 * *Files identical despite different names*

### Comparing `cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/1e_ANNOTATION_WITH_OUTDATED_MODELIZATION_WITHOUT_CONFLICTS/settings.json` & `cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/1e_ANNOTATION_WITH_OUTDATED_MODELIZATION_WITHOUT_CONFLICTS/settings.json`

 * *Files identical despite different names*

### Comparing `cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/1e_ANNOTATION_WITH_OUTDATED_MODELIZATION_WITHOUT_CONFLICTS/texts.json` & `cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/1e_ANNOTATION_WITH_OUTDATED_MODELIZATION_WITHOUT_CONFLICTS/texts.json`

 * *Files identical despite different names*

### Comparing `cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/1e_ANNOTATION_WITH_OUTDATED_MODELIZATION_WITHOUT_CONFLICTS/vectors.pkl` & `cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/1e_ANNOTATION_WITH_OUTDATED_MODELIZATION_WITHOUT_CONFLICTS/vectors.pkl`

 * *Files identical despite different names*

### Comparing `cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/1e_ANNOTATION_WITH_OUTDATED_MODELIZATION_WITHOUT_CONFLICTS/vectors_2D.json` & `cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/1e_ANNOTATION_WITH_OUTDATED_MODELIZATION_WITHOUT_CONFLICTS/vectors_2D.json`

 * *Files identical despite different names*

### Comparing `cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/1e_ANNOTATION_WITH_OUTDATED_MODELIZATION_WITHOUT_CONFLICTS/vectors_3D.json` & `cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/1e_ANNOTATION_WITH_OUTDATED_MODELIZATION_WITHOUT_CONFLICTS/vectors_3D.json`

 * *Files identical despite different names*

### Comparing `cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/1f_ANNOTATION_WITH_PENDING_MODELIZATION_WITHOUT_CONFLICTS/constraints.json` & `cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/1f_ANNOTATION_WITH_PENDING_MODELIZATION_WITHOUT_CONFLICTS/constraints.json`

 * *Files identical despite different names*

### Comparing `cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/1f_ANNOTATION_WITH_PENDING_MODELIZATION_WITHOUT_CONFLICTS/constraints_manager.pkl` & `cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/1f_ANNOTATION_WITH_PENDING_MODELIZATION_WITHOUT_CONFLICTS/constraints_manager.pkl`

 * *Files identical despite different names*

### Comparing `cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/1f_ANNOTATION_WITH_PENDING_MODELIZATION_WITHOUT_CONFLICTS/modelization.json` & `cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/1f_ANNOTATION_WITH_PENDING_MODELIZATION_WITHOUT_CONFLICTS/modelization.json`

 * *Files identical despite different names*

### Comparing `cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/1f_ANNOTATION_WITH_PENDING_MODELIZATION_WITHOUT_CONFLICTS/settings.json` & `cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/1f_ANNOTATION_WITH_PENDING_MODELIZATION_WITHOUT_CONFLICTS/settings.json`

 * *Files identical despite different names*

### Comparing `cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/1f_ANNOTATION_WITH_PENDING_MODELIZATION_WITHOUT_CONFLICTS/texts.json` & `cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/1f_ANNOTATION_WITH_PENDING_MODELIZATION_WITHOUT_CONFLICTS/texts.json`

 * *Files identical despite different names*

### Comparing `cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/1f_ANNOTATION_WITH_PENDING_MODELIZATION_WITHOUT_CONFLICTS/vectors.pkl` & `cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/1f_ANNOTATION_WITH_PENDING_MODELIZATION_WITHOUT_CONFLICTS/vectors.pkl`

 * *Files identical despite different names*

### Comparing `cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/1f_ANNOTATION_WITH_PENDING_MODELIZATION_WITHOUT_CONFLICTS/vectors_2D.json` & `cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/1f_ANNOTATION_WITH_PENDING_MODELIZATION_WITHOUT_CONFLICTS/vectors_2D.json`

 * *Files identical despite different names*

### Comparing `cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/1f_ANNOTATION_WITH_PENDING_MODELIZATION_WITHOUT_CONFLICTS/vectors_3D.json` & `cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/1f_ANNOTATION_WITH_PENDING_MODELIZATION_WITHOUT_CONFLICTS/vectors_3D.json`

 * *Files identical despite different names*

### Comparing `cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/1g_ANNOTATION_WITH_WORKING_MODELIZATION_WITHOUT_CONFLICTS/constraints.json` & `cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/1g_ANNOTATION_WITH_WORKING_MODELIZATION_WITHOUT_CONFLICTS/constraints.json`

 * *Files identical despite different names*

### Comparing `cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/1g_ANNOTATION_WITH_WORKING_MODELIZATION_WITHOUT_CONFLICTS/constraints_manager.pkl` & `cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/1g_ANNOTATION_WITH_WORKING_MODELIZATION_WITHOUT_CONFLICTS/constraints_manager.pkl`

 * *Files identical despite different names*

### Comparing `cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/1g_ANNOTATION_WITH_WORKING_MODELIZATION_WITHOUT_CONFLICTS/modelization.json` & `cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/1g_ANNOTATION_WITH_WORKING_MODELIZATION_WITHOUT_CONFLICTS/modelization.json`

 * *Files identical despite different names*

### Comparing `cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/1g_ANNOTATION_WITH_WORKING_MODELIZATION_WITHOUT_CONFLICTS/settings.json` & `cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/1g_ANNOTATION_WITH_WORKING_MODELIZATION_WITHOUT_CONFLICTS/settings.json`

 * *Files identical despite different names*

### Comparing `cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/1g_ANNOTATION_WITH_WORKING_MODELIZATION_WITHOUT_CONFLICTS/texts.json` & `cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/1g_ANNOTATION_WITH_WORKING_MODELIZATION_WITHOUT_CONFLICTS/texts.json`

 * *Files identical despite different names*

### Comparing `cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/1g_ANNOTATION_WITH_WORKING_MODELIZATION_WITHOUT_CONFLICTS/vectors.pkl` & `cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/1g_ANNOTATION_WITH_WORKING_MODELIZATION_WITHOUT_CONFLICTS/vectors.pkl`

 * *Files identical despite different names*

### Comparing `cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/1g_ANNOTATION_WITH_WORKING_MODELIZATION_WITHOUT_CONFLICTS/vectors_2D.json` & `cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/1g_ANNOTATION_WITH_WORKING_MODELIZATION_WITHOUT_CONFLICTS/vectors_2D.json`

 * *Files identical despite different names*

### Comparing `cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/1g_ANNOTATION_WITH_WORKING_MODELIZATION_WITHOUT_CONFLICTS/vectors_3D.json` & `cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/1g_ANNOTATION_WITH_WORKING_MODELIZATION_WITHOUT_CONFLICTS/vectors_3D.json`

 * *Files identical despite different names*

### Comparing `cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/1h_ANNOTATION_WITH_OUTDATED_MODELIZATION_WITH_CONFLICTS/constraints.json` & `cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/1h_ANNOTATION_WITH_OUTDATED_MODELIZATION_WITH_CONFLICTS/constraints.json`

 * *Files identical despite different names*

### Comparing `cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/1h_ANNOTATION_WITH_OUTDATED_MODELIZATION_WITH_CONFLICTS/constraints_manager.pkl` & `cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/1h_ANNOTATION_WITH_OUTDATED_MODELIZATION_WITH_CONFLICTS/constraints_manager.pkl`

 * *Files identical despite different names*

### Comparing `cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/1h_ANNOTATION_WITH_OUTDATED_MODELIZATION_WITH_CONFLICTS/modelization.json` & `cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/1h_ANNOTATION_WITH_OUTDATED_MODELIZATION_WITH_CONFLICTS/modelization.json`

 * *Files identical despite different names*

### Comparing `cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/1h_ANNOTATION_WITH_OUTDATED_MODELIZATION_WITH_CONFLICTS/settings.json` & `cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/1h_ANNOTATION_WITH_OUTDATED_MODELIZATION_WITH_CONFLICTS/settings.json`

 * *Files identical despite different names*

### Comparing `cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/1h_ANNOTATION_WITH_OUTDATED_MODELIZATION_WITH_CONFLICTS/texts.json` & `cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/1h_ANNOTATION_WITH_OUTDATED_MODELIZATION_WITH_CONFLICTS/texts.json`

 * *Files identical despite different names*

### Comparing `cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/1h_ANNOTATION_WITH_OUTDATED_MODELIZATION_WITH_CONFLICTS/vectors.pkl` & `cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/1h_ANNOTATION_WITH_OUTDATED_MODELIZATION_WITH_CONFLICTS/vectors.pkl`

 * *Files identical despite different names*

### Comparing `cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/1h_ANNOTATION_WITH_OUTDATED_MODELIZATION_WITH_CONFLICTS/vectors_2D.json` & `cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/1h_ANNOTATION_WITH_OUTDATED_MODELIZATION_WITH_CONFLICTS/vectors_2D.json`

 * *Files identical despite different names*

### Comparing `cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/1h_ANNOTATION_WITH_OUTDATED_MODELIZATION_WITH_CONFLICTS/vectors_3D.json` & `cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/1h_ANNOTATION_WITH_OUTDATED_MODELIZATION_WITH_CONFLICTS/vectors_3D.json`

 * *Files identical despite different names*

### Comparing `cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/1i_ANNOTATION_WITH_OUTDATED_MODELIZATION_WITH_CONFLICTS/constraints.json` & `cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/1i_ANNOTATION_WITH_OUTDATED_MODELIZATION_WITH_CONFLICTS/constraints.json`

 * *Files identical despite different names*

### Comparing `cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/1i_ANNOTATION_WITH_OUTDATED_MODELIZATION_WITH_CONFLICTS/constraints_manager.pkl` & `cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/1i_ANNOTATION_WITH_OUTDATED_MODELIZATION_WITH_CONFLICTS/constraints_manager.pkl`

 * *Files identical despite different names*

### Comparing `cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/1i_ANNOTATION_WITH_OUTDATED_MODELIZATION_WITH_CONFLICTS/modelization.json` & `cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/1i_ANNOTATION_WITH_OUTDATED_MODELIZATION_WITH_CONFLICTS/modelization.json`

 * *Files identical despite different names*

### Comparing `cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/1i_ANNOTATION_WITH_OUTDATED_MODELIZATION_WITH_CONFLICTS/settings.json` & `cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/1i_ANNOTATION_WITH_OUTDATED_MODELIZATION_WITH_CONFLICTS/settings.json`

 * *Files identical despite different names*

### Comparing `cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/1i_ANNOTATION_WITH_OUTDATED_MODELIZATION_WITH_CONFLICTS/texts.json` & `cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/1i_ANNOTATION_WITH_OUTDATED_MODELIZATION_WITH_CONFLICTS/texts.json`

 * *Files identical despite different names*

### Comparing `cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/1i_ANNOTATION_WITH_OUTDATED_MODELIZATION_WITH_CONFLICTS/vectors.pkl` & `cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/1i_ANNOTATION_WITH_OUTDATED_MODELIZATION_WITH_CONFLICTS/vectors.pkl`

 * *Files identical despite different names*

### Comparing `cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/1i_ANNOTATION_WITH_OUTDATED_MODELIZATION_WITH_CONFLICTS/vectors_2D.json` & `cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/1i_ANNOTATION_WITH_OUTDATED_MODELIZATION_WITH_CONFLICTS/vectors_2D.json`

 * *Files identical despite different names*

### Comparing `cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/1i_ANNOTATION_WITH_OUTDATED_MODELIZATION_WITH_CONFLICTS/vectors_3D.json` & `cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/1i_ANNOTATION_WITH_OUTDATED_MODELIZATION_WITH_CONFLICTS/vectors_3D.json`

 * *Files identical despite different names*

### Comparing `cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/1j_ANNOTATION_WITH_PENDING_MODELIZATION_WITH_CONFLICTS/constraints.json` & `cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/1j_ANNOTATION_WITH_PENDING_MODELIZATION_WITH_CONFLICTS/constraints.json`

 * *Files identical despite different names*

### Comparing `cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/1j_ANNOTATION_WITH_PENDING_MODELIZATION_WITH_CONFLICTS/constraints_manager.pkl` & `cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/1j_ANNOTATION_WITH_PENDING_MODELIZATION_WITH_CONFLICTS/constraints_manager.pkl`

 * *Files identical despite different names*

### Comparing `cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/1j_ANNOTATION_WITH_PENDING_MODELIZATION_WITH_CONFLICTS/modelization.json` & `cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/1j_ANNOTATION_WITH_PENDING_MODELIZATION_WITH_CONFLICTS/modelization.json`

 * *Files identical despite different names*

### Comparing `cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/1j_ANNOTATION_WITH_PENDING_MODELIZATION_WITH_CONFLICTS/settings.json` & `cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/1j_ANNOTATION_WITH_PENDING_MODELIZATION_WITH_CONFLICTS/settings.json`

 * *Files identical despite different names*

### Comparing `cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/1j_ANNOTATION_WITH_PENDING_MODELIZATION_WITH_CONFLICTS/texts.json` & `cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/1j_ANNOTATION_WITH_PENDING_MODELIZATION_WITH_CONFLICTS/texts.json`

 * *Files identical despite different names*

### Comparing `cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/1j_ANNOTATION_WITH_PENDING_MODELIZATION_WITH_CONFLICTS/vectors.pkl` & `cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/1j_ANNOTATION_WITH_PENDING_MODELIZATION_WITH_CONFLICTS/vectors.pkl`

 * *Files identical despite different names*

### Comparing `cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/1j_ANNOTATION_WITH_PENDING_MODELIZATION_WITH_CONFLICTS/vectors_2D.json` & `cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/1j_ANNOTATION_WITH_PENDING_MODELIZATION_WITH_CONFLICTS/vectors_2D.json`

 * *Files identical despite different names*

### Comparing `cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/1j_ANNOTATION_WITH_PENDING_MODELIZATION_WITH_CONFLICTS/vectors_3D.json` & `cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/1j_ANNOTATION_WITH_PENDING_MODELIZATION_WITH_CONFLICTS/vectors_3D.json`

 * *Files identical despite different names*

### Comparing `cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/1k_ANNOTATION_WITH_WORKING_MODELIZATION_WITH_CONFLICTS/constraints.json` & `cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/1k_ANNOTATION_WITH_WORKING_MODELIZATION_WITH_CONFLICTS/constraints.json`

 * *Files identical despite different names*

### Comparing `cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/1k_ANNOTATION_WITH_WORKING_MODELIZATION_WITH_CONFLICTS/constraints_manager.pkl` & `cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/1k_ANNOTATION_WITH_WORKING_MODELIZATION_WITH_CONFLICTS/constraints_manager.pkl`

 * *Files identical despite different names*

### Comparing `cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/1k_ANNOTATION_WITH_WORKING_MODELIZATION_WITH_CONFLICTS/modelization.json` & `cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/1k_ANNOTATION_WITH_WORKING_MODELIZATION_WITH_CONFLICTS/modelization.json`

 * *Files identical despite different names*

### Comparing `cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/1k_ANNOTATION_WITH_WORKING_MODELIZATION_WITH_CONFLICTS/settings.json` & `cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/1k_ANNOTATION_WITH_WORKING_MODELIZATION_WITH_CONFLICTS/settings.json`

 * *Files identical despite different names*

### Comparing `cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/1k_ANNOTATION_WITH_WORKING_MODELIZATION_WITH_CONFLICTS/texts.json` & `cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/1k_ANNOTATION_WITH_WORKING_MODELIZATION_WITH_CONFLICTS/texts.json`

 * *Files identical despite different names*

### Comparing `cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/1k_ANNOTATION_WITH_WORKING_MODELIZATION_WITH_CONFLICTS/vectors.pkl` & `cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/1k_ANNOTATION_WITH_WORKING_MODELIZATION_WITH_CONFLICTS/vectors.pkl`

 * *Files identical despite different names*

### Comparing `cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/1k_ANNOTATION_WITH_WORKING_MODELIZATION_WITH_CONFLICTS/vectors_2D.json` & `cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/1k_ANNOTATION_WITH_WORKING_MODELIZATION_WITH_CONFLICTS/vectors_2D.json`

 * *Files identical despite different names*

### Comparing `cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/1k_ANNOTATION_WITH_WORKING_MODELIZATION_WITH_CONFLICTS/vectors_3D.json` & `cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/1k_ANNOTATION_WITH_WORKING_MODELIZATION_WITH_CONFLICTS/vectors_3D.json`

 * *Files identical despite different names*

### Comparing `cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/1l_ANNOTATION_WITH_UPTODATE_MODELIZATION/constraints.json` & `cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/1l_ANNOTATION_WITH_UPTODATE_MODELIZATION/constraints.json`

 * *Files identical despite different names*

### Comparing `cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/1l_ANNOTATION_WITH_UPTODATE_MODELIZATION/constraints_manager.pkl` & `cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/1l_ANNOTATION_WITH_UPTODATE_MODELIZATION/constraints_manager.pkl`

 * *Files identical despite different names*

### Comparing `cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/1l_ANNOTATION_WITH_UPTODATE_MODELIZATION/modelization.json` & `cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/1l_ANNOTATION_WITH_UPTODATE_MODELIZATION/modelization.json`

 * *Files identical despite different names*

### Comparing `cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/1l_ANNOTATION_WITH_UPTODATE_MODELIZATION/settings.json` & `cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/1l_ANNOTATION_WITH_UPTODATE_MODELIZATION/settings.json`

 * *Files identical despite different names*

### Comparing `cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/1l_ANNOTATION_WITH_UPTODATE_MODELIZATION/texts.json` & `cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/1l_ANNOTATION_WITH_UPTODATE_MODELIZATION/texts.json`

 * *Files identical despite different names*

### Comparing `cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/1l_ANNOTATION_WITH_UPTODATE_MODELIZATION/vectors.pkl` & `cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/1l_ANNOTATION_WITH_UPTODATE_MODELIZATION/vectors.pkl`

 * *Files identical despite different names*

### Comparing `cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/1l_ANNOTATION_WITH_UPTODATE_MODELIZATION/vectors_2D.json` & `cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/1l_ANNOTATION_WITH_UPTODATE_MODELIZATION/vectors_2D.json`

 * *Files identical despite different names*

### Comparing `cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/1l_ANNOTATION_WITH_UPTODATE_MODELIZATION/vectors_3D.json` & `cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/1l_ANNOTATION_WITH_UPTODATE_MODELIZATION/vectors_3D.json`

 * *Files identical despite different names*

### Comparing `cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/1m_CLUSTERING_TODO/constraints.json` & `cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/1m_CLUSTERING_TODO/constraints.json`

 * *Files identical despite different names*

### Comparing `cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/1m_CLUSTERING_TODO/constraints_manager.pkl` & `cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/1m_CLUSTERING_TODO/constraints_manager.pkl`

 * *Files identical despite different names*

### Comparing `cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/1m_CLUSTERING_TODO/modelization.json` & `cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/1m_CLUSTERING_TODO/modelization.json`

 * *Files identical despite different names*

### Comparing `cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/1m_CLUSTERING_TODO/settings.json` & `cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/1m_CLUSTERING_TODO/settings.json`

 * *Files identical despite different names*

### Comparing `cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/1m_CLUSTERING_TODO/texts.json` & `cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/1m_CLUSTERING_TODO/texts.json`

 * *Files identical despite different names*

### Comparing `cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/1m_CLUSTERING_TODO/vectors.pkl` & `cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/1m_CLUSTERING_TODO/vectors.pkl`

 * *Files identical despite different names*

### Comparing `cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/1m_CLUSTERING_TODO/vectors_2D.json` & `cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/1m_CLUSTERING_TODO/vectors_2D.json`

 * *Files identical despite different names*

### Comparing `cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/1m_CLUSTERING_TODO/vectors_3D.json` & `cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/1m_CLUSTERING_TODO/vectors_3D.json`

 * *Files identical despite different names*

### Comparing `cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/1n_CLUSTERING_PENDING/constraints.json` & `cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/1n_CLUSTERING_PENDING/constraints.json`

 * *Files identical despite different names*

### Comparing `cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/1n_CLUSTERING_PENDING/constraints_manager.pkl` & `cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/1n_CLUSTERING_PENDING/constraints_manager.pkl`

 * *Files identical despite different names*

### Comparing `cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/1n_CLUSTERING_PENDING/modelization.json` & `cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/1n_CLUSTERING_PENDING/modelization.json`

 * *Files identical despite different names*

### Comparing `cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/1n_CLUSTERING_PENDING/settings.json` & `cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/1n_CLUSTERING_PENDING/settings.json`

 * *Files identical despite different names*

### Comparing `cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/1n_CLUSTERING_PENDING/texts.json` & `cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/1n_CLUSTERING_PENDING/texts.json`

 * *Files identical despite different names*

### Comparing `cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/1n_CLUSTERING_PENDING/vectors.pkl` & `cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/1n_CLUSTERING_PENDING/vectors.pkl`

 * *Files identical despite different names*

### Comparing `cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/1n_CLUSTERING_PENDING/vectors_2D.json` & `cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/1n_CLUSTERING_PENDING/vectors_2D.json`

 * *Files identical despite different names*

### Comparing `cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/1n_CLUSTERING_PENDING/vectors_3D.json` & `cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/1n_CLUSTERING_PENDING/vectors_3D.json`

 * *Files identical despite different names*

### Comparing `cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/1o_CLUSTERING_WORKING/constraints.json` & `cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/1o_CLUSTERING_WORKING/constraints.json`

 * *Files identical despite different names*

### Comparing `cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/1o_CLUSTERING_WORKING/constraints_manager.pkl` & `cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/1o_CLUSTERING_WORKING/constraints_manager.pkl`

 * *Files identical despite different names*

### Comparing `cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/1o_CLUSTERING_WORKING/modelization.json` & `cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/1o_CLUSTERING_WORKING/modelization.json`

 * *Files identical despite different names*

### Comparing `cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/1o_CLUSTERING_WORKING/settings.json` & `cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/1o_CLUSTERING_WORKING/settings.json`

 * *Files identical despite different names*

### Comparing `cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/1o_CLUSTERING_WORKING/texts.json` & `cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/1o_CLUSTERING_WORKING/texts.json`

 * *Files identical despite different names*

### Comparing `cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/1o_CLUSTERING_WORKING/vectors.pkl` & `cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/1o_CLUSTERING_WORKING/vectors.pkl`

 * *Files identical despite different names*

### Comparing `cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/1o_CLUSTERING_WORKING/vectors_2D.json` & `cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/1o_CLUSTERING_WORKING/vectors_2D.json`

 * *Files identical despite different names*

### Comparing `cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/1o_CLUSTERING_WORKING/vectors_3D.json` & `cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/1o_CLUSTERING_WORKING/vectors_3D.json`

 * *Files identical despite different names*

### Comparing `cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/1p_ITERATION_END/clustering.json` & `cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/1p_ITERATION_END/clustering.json`

 * *Files identical despite different names*

### Comparing `cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/1p_ITERATION_END/constraints.json` & `cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/1p_ITERATION_END/constraints.json`

 * *Files identical despite different names*

### Comparing `cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/1p_ITERATION_END/constraints_manager.pkl` & `cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/1p_ITERATION_END/constraints_manager.pkl`

 * *Files identical despite different names*

### Comparing `cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/1p_ITERATION_END/modelization.json` & `cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/1p_ITERATION_END/modelization.json`

 * *Files identical despite different names*

### Comparing `cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/1p_ITERATION_END/settings.json` & `cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/1p_ITERATION_END/settings.json`

 * *Files identical despite different names*

### Comparing `cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/1p_ITERATION_END/texts.json` & `cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/1p_ITERATION_END/texts.json`

 * *Files identical despite different names*

### Comparing `cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/1p_ITERATION_END/vectors.pkl` & `cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/1p_ITERATION_END/vectors.pkl`

 * *Files identical despite different names*

### Comparing `cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/1p_ITERATION_END/vectors_2D.json` & `cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/1p_ITERATION_END/vectors_2D.json`

 * *Files identical despite different names*

### Comparing `cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/1p_ITERATION_END/vectors_3D.json` & `cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/1p_ITERATION_END/vectors_3D.json`

 * *Files identical despite different names*

### Comparing `cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/2a_SAMPLING_TODO/clustering.json` & `cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/2a_SAMPLING_TODO/clustering.json`

 * *Files identical despite different names*

### Comparing `cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/2a_SAMPLING_TODO/constraints.json` & `cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/2a_SAMPLING_TODO/constraints.json`

 * *Files identical despite different names*

### Comparing `cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/2a_SAMPLING_TODO/constraints_manager.pkl` & `cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/2a_SAMPLING_TODO/constraints_manager.pkl`

 * *Files identical despite different names*

### Comparing `cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/2a_SAMPLING_TODO/modelization.json` & `cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/2a_SAMPLING_TODO/modelization.json`

 * *Files identical despite different names*

### Comparing `cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/2a_SAMPLING_TODO/settings.json` & `cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/2a_SAMPLING_TODO/settings.json`

 * *Files identical despite different names*

### Comparing `cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/2a_SAMPLING_TODO/texts.json` & `cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/2a_SAMPLING_TODO/texts.json`

 * *Files identical despite different names*

### Comparing `cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/2a_SAMPLING_TODO/vectors.pkl` & `cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/2a_SAMPLING_TODO/vectors.pkl`

 * *Files identical despite different names*

### Comparing `cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/2a_SAMPLING_TODO/vectors_2D.json` & `cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/2a_SAMPLING_TODO/vectors_2D.json`

 * *Files identical despite different names*

### Comparing `cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/2a_SAMPLING_TODO/vectors_3D.json` & `cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/2a_SAMPLING_TODO/vectors_3D.json`

 * *Files identical despite different names*

### Comparing `cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/2b2_SAMPLING_PENDING/clustering.json` & `cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/2b2_SAMPLING_PENDING/clustering.json`

 * *Files identical despite different names*

### Comparing `cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/2b2_SAMPLING_PENDING/constraints.json` & `cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/2b2_SAMPLING_PENDING/constraints.json`

 * *Files identical despite different names*

### Comparing `cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/2b2_SAMPLING_PENDING/constraints_manager.pkl` & `cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/2b2_SAMPLING_PENDING/constraints_manager.pkl`

 * *Files identical despite different names*

### Comparing `cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/2b2_SAMPLING_PENDING/modelization.json` & `cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/2b2_SAMPLING_PENDING/modelization.json`

 * *Files identical despite different names*

### Comparing `cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/2b2_SAMPLING_PENDING/settings.json` & `cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/2b2_SAMPLING_PENDING/settings.json`

 * *Files identical despite different names*

### Comparing `cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/2b2_SAMPLING_PENDING/texts.json` & `cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/2b2_SAMPLING_PENDING/texts.json`

 * *Files identical despite different names*

### Comparing `cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/2b2_SAMPLING_PENDING/vectors.pkl` & `cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/2b2_SAMPLING_PENDING/vectors.pkl`

 * *Files identical despite different names*

### Comparing `cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/2b2_SAMPLING_PENDING/vectors_2D.json` & `cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/2b2_SAMPLING_PENDING/vectors_2D.json`

 * *Files identical despite different names*

### Comparing `cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/2b2_SAMPLING_PENDING/vectors_3D.json` & `cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/2b2_SAMPLING_PENDING/vectors_3D.json`

 * *Files identical despite different names*

### Comparing `cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/2b_SAMPLING_PENDING/clustering.json` & `cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/2b_SAMPLING_PENDING/clustering.json`

 * *Files identical despite different names*

### Comparing `cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/2b_SAMPLING_PENDING/constraints.json` & `cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/2b_SAMPLING_PENDING/constraints.json`

 * *Files identical despite different names*

### Comparing `cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/2b_SAMPLING_PENDING/constraints_manager.pkl` & `cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/2b_SAMPLING_PENDING/constraints_manager.pkl`

 * *Files identical despite different names*

### Comparing `cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/2b_SAMPLING_PENDING/modelization.json` & `cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/2b_SAMPLING_PENDING/modelization.json`

 * *Files identical despite different names*

### Comparing `cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/2b_SAMPLING_PENDING/settings.json` & `cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/2b_SAMPLING_PENDING/settings.json`

 * *Files identical despite different names*

### Comparing `cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/2b_SAMPLING_PENDING/texts.json` & `cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/2b_SAMPLING_PENDING/texts.json`

 * *Files identical despite different names*

### Comparing `cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/2b_SAMPLING_PENDING/vectors.pkl` & `cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/2b_SAMPLING_PENDING/vectors.pkl`

 * *Files identical despite different names*

### Comparing `cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/2b_SAMPLING_PENDING/vectors_2D.json` & `cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/2b_SAMPLING_PENDING/vectors_2D.json`

 * *Files identical despite different names*

### Comparing `cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/2b_SAMPLING_PENDING/vectors_3D.json` & `cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/2b_SAMPLING_PENDING/vectors_3D.json`

 * *Files identical despite different names*

### Comparing `cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/2d_ANNOTATION_WITH_UPTODATE_MODELIZATION/clustering.json` & `cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/2d_ANNOTATION_WITH_UPTODATE_MODELIZATION/clustering.json`

 * *Files identical despite different names*

### Comparing `cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/2d_ANNOTATION_WITH_UPTODATE_MODELIZATION/constraints.json` & `cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/2d_ANNOTATION_WITH_UPTODATE_MODELIZATION/constraints.json`

 * *Files identical despite different names*

### Comparing `cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/2d_ANNOTATION_WITH_UPTODATE_MODELIZATION/constraints_manager.pkl` & `cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/2d_ANNOTATION_WITH_UPTODATE_MODELIZATION/constraints_manager.pkl`

 * *Files identical despite different names*

### Comparing `cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/2d_ANNOTATION_WITH_UPTODATE_MODELIZATION/modelization.json` & `cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/2d_ANNOTATION_WITH_UPTODATE_MODELIZATION/modelization.json`

 * *Files identical despite different names*

### Comparing `cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/2d_ANNOTATION_WITH_UPTODATE_MODELIZATION/sampling.json` & `cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/2d_ANNOTATION_WITH_UPTODATE_MODELIZATION/sampling.json`

 * *Files identical despite different names*

### Comparing `cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/2d_ANNOTATION_WITH_UPTODATE_MODELIZATION/settings.json` & `cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/2d_ANNOTATION_WITH_UPTODATE_MODELIZATION/settings.json`

 * *Files identical despite different names*

### Comparing `cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/2d_ANNOTATION_WITH_UPTODATE_MODELIZATION/texts.json` & `cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/2d_ANNOTATION_WITH_UPTODATE_MODELIZATION/texts.json`

 * *Files identical despite different names*

### Comparing `cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/2d_ANNOTATION_WITH_UPTODATE_MODELIZATION/vectors.pkl` & `cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/2d_ANNOTATION_WITH_UPTODATE_MODELIZATION/vectors.pkl`

 * *Files identical despite different names*

### Comparing `cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/2d_ANNOTATION_WITH_UPTODATE_MODELIZATION/vectors_2D.json` & `cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/2d_ANNOTATION_WITH_UPTODATE_MODELIZATION/vectors_2D.json`

 * *Files identical despite different names*

### Comparing `cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/2d_ANNOTATION_WITH_UPTODATE_MODELIZATION/vectors_3D.json` & `cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/2d_ANNOTATION_WITH_UPTODATE_MODELIZATION/vectors_3D.json`

 * *Files identical despite different names*

### Comparing `cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/archive-0a_INITIALIZATION_WITHOUT_MODELIZATION.zip` & `cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/archive-0a_INITIALIZATION_WITHOUT_MODELIZATION.zip`

 * *Files identical despite different names*

### Comparing `cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/archive-1b_SAMPLING_PENDING.zip` & `cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/archive-1b_SAMPLING_PENDING.zip`

 * *Files identical despite different names*

### Comparing `cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/archive-1d_ANNOTATION_WITH_UPTODATE_MODELIZATION.zip` & `cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/archive-1d_ANNOTATION_WITH_UPTODATE_MODELIZATION.zip`

 * *Files identical despite different names*

### Comparing `cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/archive-1h_ANNOTATION_WITH_OUTDATED_MODELIZATION_WITH_CONFLICTS.zip` & `cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/archive-1h_ANNOTATION_WITH_OUTDATED_MODELIZATION_WITH_CONFLICTS.zip`

 * *Files identical despite different names*

### Comparing `cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/archive-1j_ANNOTATION_WITH_PENDING_MODELIZATION_WITH_CONFLICTS.zip` & `cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/archive-1j_ANNOTATION_WITH_PENDING_MODELIZATION_WITH_CONFLICTS.zip`

 * *Files identical despite different names*

### Comparing `cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/archive-1l_ANNOTATION_WITH_UPTODATE_MODELIZATION.zip` & `cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/archive-1l_ANNOTATION_WITH_UPTODATE_MODELIZATION.zip`

 * *Files identical despite different names*

### Comparing `cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/archive-1o_CLUSTERING_WORKING.zip` & `cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/archive-1o_CLUSTERING_WORKING.zip`

 * *Files identical despite different names*

### Comparing `cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/archive-1p_ITERATION_END.zip` & `cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/archive-1p_ITERATION_END.zip`

 * *Files identical despite different names*

### Comparing `cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/archive-ERROR_bad_archive.zip` & `cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/archive-ERROR_bad_archive.zip`

 * *Files identical despite different names*

### Comparing `cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/archive-ERROR_metadata_bad_creation_timestamp.zip` & `cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/archive-ERROR_metadata_bad_creation_timestamp.zip`

 * *Files identical despite different names*

### Comparing `cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/archive-ERROR_metadata_bad_project_name.zip` & `cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/archive-ERROR_metadata_bad_project_name.zip`

 * *Files identical despite different names*

### Comparing `cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/archive-ERROR_metadata_missing_creation_timestamp.zip` & `cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/archive-ERROR_metadata_missing_creation_timestamp.zip`

 * *Files identical despite different names*

### Comparing `cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/archive-ERROR_metadata_missing_project_name.zip` & `cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/archive-ERROR_metadata_missing_project_name.zip`

 * *Files identical despite different names*

### Comparing `cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/archive-ERROR_missing_files.zip` & `cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/archive-ERROR_missing_files.zip`

 * *Files identical despite different names*

### Comparing `cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/archive-ERROR_status_bad_state.zip` & `cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/archive-ERROR_status_bad_state.zip`

 * *Files identical despite different names*

### Comparing `cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/archive-ERROR_status_missing_state.zip` & `cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/archive-ERROR_status_missing_state.zip`

 * *Files identical despite different names*

### Comparing `cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/dummy_24.csv` & `cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/dummy_24.csv`

 * *Files identical despite different names*

### Comparing `cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/dummy_24.txt` & `cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/dummy_24.txt`

 * *Files identical despite different names*

### Comparing `cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/dummy_24.xlsx` & `cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/dummy_24.xlsx`

 * *Files identical despite different names*

### Comparing `cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/dummy_24_err.csv` & `cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/dummy_24_err.csv`

 * *Files identical despite different names*

### Comparing `cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/dummy_24_err.xlsx` & `cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/dummy_24_err.xlsx`

 * *Files identical despite different names*

### Comparing `cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/import_0y0_INITIALIZATION_WITHOUT_MODELIZATION/modelization.json` & `cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/import_0y0_INITIALIZATION_WITHOUT_MODELIZATION/modelization.json`

 * *Files identical despite different names*

### Comparing `cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/import_0y0_INITIALIZATION_WITHOUT_MODELIZATION/settings.json` & `cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/import_0y0_INITIALIZATION_WITHOUT_MODELIZATION/settings.json`

 * *Files identical despite different names*

### Comparing `cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/import_0y0_INITIALIZATION_WITHOUT_MODELIZATION/texts.json` & `cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/import_0y0_INITIALIZATION_WITHOUT_MODELIZATION/texts.json`

 * *Files identical despite different names*

### Comparing `cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/import_0y1_INITIALIZATION_WITH_PENDING_MODELIZATION/modelization.json` & `cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/import_0y1_INITIALIZATION_WITH_PENDING_MODELIZATION/modelization.json`

 * *Files identical despite different names*

### Comparing `cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/import_0y1_INITIALIZATION_WITH_PENDING_MODELIZATION/settings.json` & `cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/import_0y1_INITIALIZATION_WITH_PENDING_MODELIZATION/settings.json`

 * *Files identical despite different names*

### Comparing `cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/import_0y1_INITIALIZATION_WITH_PENDING_MODELIZATION/texts.json` & `cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/import_0y1_INITIALIZATION_WITH_PENDING_MODELIZATION/texts.json`

 * *Files identical despite different names*

### Comparing `cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/import_0y2_INITIALIZATION_WITH_WORKING_MODELIZATION/modelization.json` & `cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/import_0y2_INITIALIZATION_WITH_WORKING_MODELIZATION/modelization.json`

 * *Files identical despite different names*

### Comparing `cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/import_0y2_INITIALIZATION_WITH_WORKING_MODELIZATION/settings.json` & `cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/import_0y2_INITIALIZATION_WITH_WORKING_MODELIZATION/settings.json`

 * *Files identical despite different names*

### Comparing `cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/import_0y2_INITIALIZATION_WITH_WORKING_MODELIZATION/texts.json` & `cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/import_0y2_INITIALIZATION_WITH_WORKING_MODELIZATION/texts.json`

 * *Files identical despite different names*

### Comparing `cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/import_1w0_IMPORT_AT_SAMPLING_STEP_WITHOUT_MODELIZATION/modelization.json` & `cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/import_1w0_IMPORT_AT_SAMPLING_STEP_WITHOUT_MODELIZATION/modelization.json`

 * *Files identical despite different names*

### Comparing `cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/import_1w0_IMPORT_AT_SAMPLING_STEP_WITHOUT_MODELIZATION/settings.json` & `cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/import_1w0_IMPORT_AT_SAMPLING_STEP_WITHOUT_MODELIZATION/settings.json`

 * *Files identical despite different names*

### Comparing `cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/import_1w0_IMPORT_AT_SAMPLING_STEP_WITHOUT_MODELIZATION/texts.json` & `cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/import_1w0_IMPORT_AT_SAMPLING_STEP_WITHOUT_MODELIZATION/texts.json`

 * *Files identical despite different names*

### Comparing `cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/import_1w1_IMPORT_AT_SAMPLING_STEP_WITH_PENDING_MODELIZATION/modelization.json` & `cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/import_1w1_IMPORT_AT_SAMPLING_STEP_WITH_PENDING_MODELIZATION/modelization.json`

 * *Files identical despite different names*

### Comparing `cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/import_1w1_IMPORT_AT_SAMPLING_STEP_WITH_PENDING_MODELIZATION/settings.json` & `cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/import_1w1_IMPORT_AT_SAMPLING_STEP_WITH_PENDING_MODELIZATION/settings.json`

 * *Files identical despite different names*

### Comparing `cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/import_1w1_IMPORT_AT_SAMPLING_STEP_WITH_PENDING_MODELIZATION/texts.json` & `cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/import_1w1_IMPORT_AT_SAMPLING_STEP_WITH_PENDING_MODELIZATION/texts.json`

 * *Files identical despite different names*

### Comparing `cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/import_1w2_IMPORT_AT_SAMPLING_STEP_WORKING_MODELIZATION/modelization.json` & `cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/import_1w2_IMPORT_AT_SAMPLING_STEP_WORKING_MODELIZATION/modelization.json`

 * *Files identical despite different names*

### Comparing `cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/import_1w2_IMPORT_AT_SAMPLING_STEP_WORKING_MODELIZATION/settings.json` & `cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/import_1w2_IMPORT_AT_SAMPLING_STEP_WORKING_MODELIZATION/settings.json`

 * *Files identical despite different names*

### Comparing `cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/import_1w2_IMPORT_AT_SAMPLING_STEP_WORKING_MODELIZATION/texts.json` & `cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/import_1w2_IMPORT_AT_SAMPLING_STEP_WORKING_MODELIZATION/texts.json`

 * *Files identical despite different names*

### Comparing `cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/import_1x0_IMPORT_AT_ANNOTATION_STEP_WITHOUT_MODELIZATION/constraints.json` & `cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/import_1x0_IMPORT_AT_ANNOTATION_STEP_WITHOUT_MODELIZATION/constraints.json`

 * *Files identical despite different names*

### Comparing `cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/import_1x0_IMPORT_AT_ANNOTATION_STEP_WITHOUT_MODELIZATION/modelization.json` & `cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/import_1x0_IMPORT_AT_ANNOTATION_STEP_WITHOUT_MODELIZATION/modelization.json`

 * *Files identical despite different names*

### Comparing `cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/import_1x0_IMPORT_AT_ANNOTATION_STEP_WITHOUT_MODELIZATION/settings.json` & `cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/import_1x0_IMPORT_AT_ANNOTATION_STEP_WITHOUT_MODELIZATION/settings.json`

 * *Files identical despite different names*

### Comparing `cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/import_1x0_IMPORT_AT_ANNOTATION_STEP_WITHOUT_MODELIZATION/texts.json` & `cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/import_1x0_IMPORT_AT_ANNOTATION_STEP_WITHOUT_MODELIZATION/texts.json`

 * *Files identical despite different names*

### Comparing `cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/import_1x1_IMPORT_AT_ANNOTATION_STEP_WITH_PENDING_MODELIZATION/constraints.json` & `cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/import_1x1_IMPORT_AT_ANNOTATION_STEP_WITH_PENDING_MODELIZATION/constraints.json`

 * *Files identical despite different names*

### Comparing `cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/import_1x1_IMPORT_AT_ANNOTATION_STEP_WITH_PENDING_MODELIZATION/modelization.json` & `cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/import_1x1_IMPORT_AT_ANNOTATION_STEP_WITH_PENDING_MODELIZATION/modelization.json`

 * *Files identical despite different names*

### Comparing `cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/import_1x1_IMPORT_AT_ANNOTATION_STEP_WITH_PENDING_MODELIZATION/settings.json` & `cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/import_1x1_IMPORT_AT_ANNOTATION_STEP_WITH_PENDING_MODELIZATION/settings.json`

 * *Files identical despite different names*

### Comparing `cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/import_1x1_IMPORT_AT_ANNOTATION_STEP_WITH_PENDING_MODELIZATION/texts.json` & `cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/import_1x1_IMPORT_AT_ANNOTATION_STEP_WITH_PENDING_MODELIZATION/texts.json`

 * *Files identical despite different names*

### Comparing `cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/import_1x2_IMPORT_AT_ANNOTATION_STEP_WORKING_MODELIZATION/constraints.json` & `cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/import_1x2_IMPORT_AT_ANNOTATION_STEP_WORKING_MODELIZATION/constraints.json`

 * *Files identical despite different names*

### Comparing `cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/import_1x2_IMPORT_AT_ANNOTATION_STEP_WORKING_MODELIZATION/modelization.json` & `cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/import_1x2_IMPORT_AT_ANNOTATION_STEP_WORKING_MODELIZATION/modelization.json`

 * *Files identical despite different names*

### Comparing `cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/import_1x2_IMPORT_AT_ANNOTATION_STEP_WORKING_MODELIZATION/settings.json` & `cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/import_1x2_IMPORT_AT_ANNOTATION_STEP_WORKING_MODELIZATION/settings.json`

 * *Files identical despite different names*

### Comparing `cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/import_1x2_IMPORT_AT_ANNOTATION_STEP_WORKING_MODELIZATION/texts.json` & `cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/import_1x2_IMPORT_AT_ANNOTATION_STEP_WORKING_MODELIZATION/texts.json`

 * *Files identical despite different names*

### Comparing `cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/import_1y0_IMPORT_AT_CLUSTERING_STEP_WITHOUT_MODELIZATION/constraints.json` & `cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/import_1y0_IMPORT_AT_CLUSTERING_STEP_WITHOUT_MODELIZATION/constraints.json`

 * *Files identical despite different names*

### Comparing `cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/import_1y0_IMPORT_AT_CLUSTERING_STEP_WITHOUT_MODELIZATION/modelization.json` & `cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/import_1y0_IMPORT_AT_CLUSTERING_STEP_WITHOUT_MODELIZATION/modelization.json`

 * *Files identical despite different names*

### Comparing `cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/import_1y0_IMPORT_AT_CLUSTERING_STEP_WITHOUT_MODELIZATION/settings.json` & `cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/import_1y0_IMPORT_AT_CLUSTERING_STEP_WITHOUT_MODELIZATION/settings.json`

 * *Files identical despite different names*

### Comparing `cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/import_1y0_IMPORT_AT_CLUSTERING_STEP_WITHOUT_MODELIZATION/texts.json` & `cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/import_1y0_IMPORT_AT_CLUSTERING_STEP_WITHOUT_MODELIZATION/texts.json`

 * *Files identical despite different names*

### Comparing `cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/import_1y1_IMPORT_AT_CLUSTERING_STEP_WITH_PENDING_MODELIZATION/constraints.json` & `cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/import_1y1_IMPORT_AT_CLUSTERING_STEP_WITH_PENDING_MODELIZATION/constraints.json`

 * *Files identical despite different names*

### Comparing `cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/import_1y1_IMPORT_AT_CLUSTERING_STEP_WITH_PENDING_MODELIZATION/modelization.json` & `cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/import_1y1_IMPORT_AT_CLUSTERING_STEP_WITH_PENDING_MODELIZATION/modelization.json`

 * *Files identical despite different names*

### Comparing `cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/import_1y1_IMPORT_AT_CLUSTERING_STEP_WITH_PENDING_MODELIZATION/settings.json` & `cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/import_1y1_IMPORT_AT_CLUSTERING_STEP_WITH_PENDING_MODELIZATION/settings.json`

 * *Files identical despite different names*

### Comparing `cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/import_1y1_IMPORT_AT_CLUSTERING_STEP_WITH_PENDING_MODELIZATION/texts.json` & `cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/import_1y1_IMPORT_AT_CLUSTERING_STEP_WITH_PENDING_MODELIZATION/texts.json`

 * *Files identical despite different names*

### Comparing `cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/import_1y2_IMPORT_AT_CLUSTERING_STEP_WORKING_MODELIZATION/constraints.json` & `cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/import_1y2_IMPORT_AT_CLUSTERING_STEP_WORKING_MODELIZATION/constraints.json`

 * *Files identical despite different names*

### Comparing `cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/import_1y2_IMPORT_AT_CLUSTERING_STEP_WORKING_MODELIZATION/modelization.json` & `cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/import_1y2_IMPORT_AT_CLUSTERING_STEP_WORKING_MODELIZATION/modelization.json`

 * *Files identical despite different names*

### Comparing `cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/import_1y2_IMPORT_AT_CLUSTERING_STEP_WORKING_MODELIZATION/settings.json` & `cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/import_1y2_IMPORT_AT_CLUSTERING_STEP_WORKING_MODELIZATION/settings.json`

 * *Files identical despite different names*

### Comparing `cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/import_1y2_IMPORT_AT_CLUSTERING_STEP_WORKING_MODELIZATION/texts.json` & `cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/import_1y2_IMPORT_AT_CLUSTERING_STEP_WORKING_MODELIZATION/texts.json`

 * *Files identical despite different names*

### Comparing `cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/import_1z0_IMPORT_AT_ITERATION_END_WITHOUT_MODELIZATION/clustering.json` & `cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/import_1z0_IMPORT_AT_ITERATION_END_WITHOUT_MODELIZATION/clustering.json`

 * *Files identical despite different names*

### Comparing `cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/import_1z0_IMPORT_AT_ITERATION_END_WITHOUT_MODELIZATION/constraints.json` & `cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/import_1z0_IMPORT_AT_ITERATION_END_WITHOUT_MODELIZATION/constraints.json`

 * *Files identical despite different names*

### Comparing `cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/import_1z0_IMPORT_AT_ITERATION_END_WITHOUT_MODELIZATION/modelization.json` & `cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/import_1z0_IMPORT_AT_ITERATION_END_WITHOUT_MODELIZATION/modelization.json`

 * *Files identical despite different names*

### Comparing `cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/import_1z0_IMPORT_AT_ITERATION_END_WITHOUT_MODELIZATION/settings.json` & `cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/import_1z0_IMPORT_AT_ITERATION_END_WITHOUT_MODELIZATION/settings.json`

 * *Files identical despite different names*

### Comparing `cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/import_1z0_IMPORT_AT_ITERATION_END_WITHOUT_MODELIZATION/texts.json` & `cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/import_1z0_IMPORT_AT_ITERATION_END_WITHOUT_MODELIZATION/texts.json`

 * *Files identical despite different names*

### Comparing `cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/import_1z1_IMPORT_AT_ITERATION_END_WITH_PENDING_MODELIZATION/clustering.json` & `cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/import_1z1_IMPORT_AT_ITERATION_END_WITH_PENDING_MODELIZATION/clustering.json`

 * *Files identical despite different names*

### Comparing `cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/import_1z1_IMPORT_AT_ITERATION_END_WITH_PENDING_MODELIZATION/constraints.json` & `cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/import_1z1_IMPORT_AT_ITERATION_END_WITH_PENDING_MODELIZATION/constraints.json`

 * *Files identical despite different names*

### Comparing `cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/import_1z1_IMPORT_AT_ITERATION_END_WITH_PENDING_MODELIZATION/modelization.json` & `cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/import_1z1_IMPORT_AT_ITERATION_END_WITH_PENDING_MODELIZATION/modelization.json`

 * *Files identical despite different names*

### Comparing `cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/import_1z1_IMPORT_AT_ITERATION_END_WITH_PENDING_MODELIZATION/settings.json` & `cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/import_1z1_IMPORT_AT_ITERATION_END_WITH_PENDING_MODELIZATION/settings.json`

 * *Files identical despite different names*

### Comparing `cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/import_1z1_IMPORT_AT_ITERATION_END_WITH_PENDING_MODELIZATION/texts.json` & `cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/import_1z1_IMPORT_AT_ITERATION_END_WITH_PENDING_MODELIZATION/texts.json`

 * *Files identical despite different names*

### Comparing `cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/import_1z2_IMPORT_AT_ITERATION_END_WORKING_MODELIZATION/clustering.json` & `cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/import_1z2_IMPORT_AT_ITERATION_END_WORKING_MODELIZATION/clustering.json`

 * *Files identical despite different names*

### Comparing `cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/import_1z2_IMPORT_AT_ITERATION_END_WORKING_MODELIZATION/constraints.json` & `cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/import_1z2_IMPORT_AT_ITERATION_END_WORKING_MODELIZATION/constraints.json`

 * *Files identical despite different names*

### Comparing `cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/import_1z2_IMPORT_AT_ITERATION_END_WORKING_MODELIZATION/modelization.json` & `cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/import_1z2_IMPORT_AT_ITERATION_END_WORKING_MODELIZATION/modelization.json`

 * *Files identical despite different names*

### Comparing `cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/import_1z2_IMPORT_AT_ITERATION_END_WORKING_MODELIZATION/settings.json` & `cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/import_1z2_IMPORT_AT_ITERATION_END_WORKING_MODELIZATION/settings.json`

 * *Files identical despite different names*

### Comparing `cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/import_1z2_IMPORT_AT_ITERATION_END_WORKING_MODELIZATION/texts.json` & `cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/import_1z2_IMPORT_AT_ITERATION_END_WORKING_MODELIZATION/texts.json`

 * *Files identical despite different names*

### Comparing `cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/import_error_0y1_INITIALIZATION_WITH_PENDING_MODELIZATION/constraints.json` & `cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/import_error_0y1_INITIALIZATION_WITH_PENDING_MODELIZATION/constraints.json`

 * *Files identical despite different names*

### Comparing `cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/import_error_0y1_INITIALIZATION_WITH_PENDING_MODELIZATION/modelization.json` & `cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/import_error_0y1_INITIALIZATION_WITH_PENDING_MODELIZATION/modelization.json`

 * *Files identical despite different names*

### Comparing `cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/import_error_0y1_INITIALIZATION_WITH_PENDING_MODELIZATION/settings.json` & `cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/import_error_0y1_INITIALIZATION_WITH_PENDING_MODELIZATION/settings.json`

 * *Files identical despite different names*

### Comparing `cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/import_error_0y1_INITIALIZATION_WITH_PENDING_MODELIZATION/texts.json` & `cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/import_error_0y1_INITIALIZATION_WITH_PENDING_MODELIZATION/texts.json`

 * *Files identical despite different names*

### Comparing `cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/import_error_0y3_INITIALIZATION_WITH_ERRORS/constraints.json` & `cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/import_error_0y3_INITIALIZATION_WITH_ERRORS/constraints.json`

 * *Files identical despite different names*

### Comparing `cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/import_error_0y3_INITIALIZATION_WITH_ERRORS/constraints_manager.pkl` & `cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/import_error_0y3_INITIALIZATION_WITH_ERRORS/constraints_manager.pkl`

 * *Files identical despite different names*

### Comparing `cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/import_error_0y3_INITIALIZATION_WITH_ERRORS/modelization.json` & `cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/import_error_0y3_INITIALIZATION_WITH_ERRORS/modelization.json`

 * *Files identical despite different names*

### Comparing `cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/import_error_0y3_INITIALIZATION_WITH_ERRORS/settings.json` & `cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/import_error_0y3_INITIALIZATION_WITH_ERRORS/settings.json`

 * *Files identical despite different names*

### Comparing `cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/import_error_0y3_INITIALIZATION_WITH_ERRORS/texts.json` & `cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/import_error_0y3_INITIALIZATION_WITH_ERRORS/texts.json`

 * *Files identical despite different names*

### Comparing `cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/import_error_0y3_INITIALIZATION_WITH_ERRORS/vectors.pkl` & `cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/import_error_0y3_INITIALIZATION_WITH_ERRORS/vectors.pkl`

 * *Files identical despite different names*

### Comparing `cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/import_error_0y3_INITIALIZATION_WITH_ERRORS/vectors_2D.json` & `cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/import_error_0y3_INITIALIZATION_WITH_ERRORS/vectors_2D.json`

 * *Files identical despite different names*

### Comparing `cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/import_error_0y3_INITIALIZATION_WITH_ERRORS/vectors_3D.json` & `cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/import_error_0y3_INITIALIZATION_WITH_ERRORS/vectors_3D.json`

 * *Files identical despite different names*

### Comparing `cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/import_error_1w1_IMPORT_AT_SAMPLING_STEP_WITH_PENDING_MODELIZATION/constraints.json` & `cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/import_error_1w1_IMPORT_AT_SAMPLING_STEP_WITH_PENDING_MODELIZATION/constraints.json`

 * *Files identical despite different names*

### Comparing `cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/import_error_1w1_IMPORT_AT_SAMPLING_STEP_WITH_PENDING_MODELIZATION/modelization.json` & `cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/import_error_1w1_IMPORT_AT_SAMPLING_STEP_WITH_PENDING_MODELIZATION/modelization.json`

 * *Files identical despite different names*

### Comparing `cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/import_error_1w1_IMPORT_AT_SAMPLING_STEP_WITH_PENDING_MODELIZATION/settings.json` & `cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/import_error_1w1_IMPORT_AT_SAMPLING_STEP_WITH_PENDING_MODELIZATION/settings.json`

 * *Files identical despite different names*

### Comparing `cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/import_error_1w1_IMPORT_AT_SAMPLING_STEP_WITH_PENDING_MODELIZATION/texts.json` & `cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/import_error_1w1_IMPORT_AT_SAMPLING_STEP_WITH_PENDING_MODELIZATION/texts.json`

 * *Files identical despite different names*

### Comparing `cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/import_error_1w3_IMPORT_AT_SAMPLING_STEP_WITH_ERRORS/constraints.json` & `cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/import_error_1w3_IMPORT_AT_SAMPLING_STEP_WITH_ERRORS/constraints.json`

 * *Files identical despite different names*

### Comparing `cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/import_error_1w3_IMPORT_AT_SAMPLING_STEP_WITH_ERRORS/constraints_manager.pkl` & `cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/import_error_1w3_IMPORT_AT_SAMPLING_STEP_WITH_ERRORS/constraints_manager.pkl`

 * *Files identical despite different names*

### Comparing `cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/import_error_1w3_IMPORT_AT_SAMPLING_STEP_WITH_ERRORS/modelization.json` & `cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/import_error_1w3_IMPORT_AT_SAMPLING_STEP_WITH_ERRORS/modelization.json`

 * *Files identical despite different names*

### Comparing `cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/import_error_1w3_IMPORT_AT_SAMPLING_STEP_WITH_ERRORS/settings.json` & `cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/import_error_1w3_IMPORT_AT_SAMPLING_STEP_WITH_ERRORS/settings.json`

 * *Files identical despite different names*

### Comparing `cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/import_error_1w3_IMPORT_AT_SAMPLING_STEP_WITH_ERRORS/texts.json` & `cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/import_error_1w3_IMPORT_AT_SAMPLING_STEP_WITH_ERRORS/texts.json`

 * *Files identical despite different names*

### Comparing `cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/import_error_1w3_IMPORT_AT_SAMPLING_STEP_WITH_ERRORS/vectors.pkl` & `cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/import_error_1w3_IMPORT_AT_SAMPLING_STEP_WITH_ERRORS/vectors.pkl`

 * *Files identical despite different names*

### Comparing `cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/import_error_1w3_IMPORT_AT_SAMPLING_STEP_WITH_ERRORS/vectors_2D.json` & `cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/import_error_1w3_IMPORT_AT_SAMPLING_STEP_WITH_ERRORS/vectors_2D.json`

 * *Files identical despite different names*

### Comparing `cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/import_error_1w3_IMPORT_AT_SAMPLING_STEP_WITH_ERRORS/vectors_3D.json` & `cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/import_error_1w3_IMPORT_AT_SAMPLING_STEP_WITH_ERRORS/vectors_3D.json`

 * *Files identical despite different names*

### Comparing `cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/import_error_1x1_IMPORT_AT_ANNOTATION_STEP_WITH_PENDING_MODELIZATION/constraints.json` & `cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/import_error_1x1_IMPORT_AT_ANNOTATION_STEP_WITH_PENDING_MODELIZATION/constraints.json`

 * *Files identical despite different names*

### Comparing `cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/import_error_1x1_IMPORT_AT_ANNOTATION_STEP_WITH_PENDING_MODELIZATION/modelization.json` & `cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/import_error_1x1_IMPORT_AT_ANNOTATION_STEP_WITH_PENDING_MODELIZATION/modelization.json`

 * *Files identical despite different names*

### Comparing `cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/import_error_1x1_IMPORT_AT_ANNOTATION_STEP_WITH_PENDING_MODELIZATION/settings.json` & `cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/import_error_1x1_IMPORT_AT_ANNOTATION_STEP_WITH_PENDING_MODELIZATION/settings.json`

 * *Files identical despite different names*

### Comparing `cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/import_error_1x1_IMPORT_AT_ANNOTATION_STEP_WITH_PENDING_MODELIZATION/texts.json` & `cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/import_error_1x1_IMPORT_AT_ANNOTATION_STEP_WITH_PENDING_MODELIZATION/texts.json`

 * *Files identical despite different names*

### Comparing `cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/import_error_1x3_ANNOTATION_WITH_OUTDATED_MODELIZATION_WITH_CONFLICTS/constraints.json` & `cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/import_error_1x3_ANNOTATION_WITH_OUTDATED_MODELIZATION_WITH_CONFLICTS/constraints.json`

 * *Files identical despite different names*

### Comparing `cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/import_error_1x3_ANNOTATION_WITH_OUTDATED_MODELIZATION_WITH_CONFLICTS/constraints_manager.pkl` & `cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/import_error_1x3_ANNOTATION_WITH_OUTDATED_MODELIZATION_WITH_CONFLICTS/constraints_manager.pkl`

 * *Files identical despite different names*

### Comparing `cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/import_error_1x3_ANNOTATION_WITH_OUTDATED_MODELIZATION_WITH_CONFLICTS/modelization.json` & `cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/import_error_1x3_ANNOTATION_WITH_OUTDATED_MODELIZATION_WITH_CONFLICTS/modelization.json`

 * *Files identical despite different names*

### Comparing `cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/import_error_1x3_ANNOTATION_WITH_OUTDATED_MODELIZATION_WITH_CONFLICTS/settings.json` & `cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/import_error_1x3_ANNOTATION_WITH_OUTDATED_MODELIZATION_WITH_CONFLICTS/settings.json`

 * *Files identical despite different names*

### Comparing `cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/import_error_1x3_ANNOTATION_WITH_OUTDATED_MODELIZATION_WITH_CONFLICTS/texts.json` & `cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/import_error_1x3_ANNOTATION_WITH_OUTDATED_MODELIZATION_WITH_CONFLICTS/texts.json`

 * *Files identical despite different names*

### Comparing `cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/import_error_1x3_ANNOTATION_WITH_OUTDATED_MODELIZATION_WITH_CONFLICTS/vectors.pkl` & `cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/import_error_1x3_ANNOTATION_WITH_OUTDATED_MODELIZATION_WITH_CONFLICTS/vectors.pkl`

 * *Files identical despite different names*

### Comparing `cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/import_error_1x3_ANNOTATION_WITH_OUTDATED_MODELIZATION_WITH_CONFLICTS/vectors_2D.json` & `cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/import_error_1x3_ANNOTATION_WITH_OUTDATED_MODELIZATION_WITH_CONFLICTS/vectors_2D.json`

 * *Files identical despite different names*

### Comparing `cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/import_error_1x3_ANNOTATION_WITH_OUTDATED_MODELIZATION_WITH_CONFLICTS/vectors_3D.json` & `cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/import_error_1x3_ANNOTATION_WITH_OUTDATED_MODELIZATION_WITH_CONFLICTS/vectors_3D.json`

 * *Files identical despite different names*

### Comparing `cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/import_error_1y1_IMPORT_AT_CLUSTERING_STEP_WITH_PENDING_MODELIZATION/constraints.json` & `cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/import_error_1y1_IMPORT_AT_CLUSTERING_STEP_WITH_PENDING_MODELIZATION/constraints.json`

 * *Files identical despite different names*

### Comparing `cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/import_error_1y1_IMPORT_AT_CLUSTERING_STEP_WITH_PENDING_MODELIZATION/modelization.json` & `cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/import_error_1y1_IMPORT_AT_CLUSTERING_STEP_WITH_PENDING_MODELIZATION/modelization.json`

 * *Files identical despite different names*

### Comparing `cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/import_error_1y1_IMPORT_AT_CLUSTERING_STEP_WITH_PENDING_MODELIZATION/settings.json` & `cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/import_error_1y1_IMPORT_AT_CLUSTERING_STEP_WITH_PENDING_MODELIZATION/settings.json`

 * *Files identical despite different names*

### Comparing `cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/import_error_1y1_IMPORT_AT_CLUSTERING_STEP_WITH_PENDING_MODELIZATION/texts.json` & `cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/import_error_1y1_IMPORT_AT_CLUSTERING_STEP_WITH_PENDING_MODELIZATION/texts.json`

 * *Files identical despite different names*

### Comparing `cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/import_error_1y3_IMPORT_AT_CLUSTERING_STEP_WITH_ERRORS/constraints.json` & `cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/import_error_1y3_IMPORT_AT_CLUSTERING_STEP_WITH_ERRORS/constraints.json`

 * *Files identical despite different names*

### Comparing `cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/import_error_1y3_IMPORT_AT_CLUSTERING_STEP_WITH_ERRORS/constraints_manager.pkl` & `cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/import_error_1y3_IMPORT_AT_CLUSTERING_STEP_WITH_ERRORS/constraints_manager.pkl`

 * *Files identical despite different names*

### Comparing `cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/import_error_1y3_IMPORT_AT_CLUSTERING_STEP_WITH_ERRORS/modelization.json` & `cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/import_error_1y3_IMPORT_AT_CLUSTERING_STEP_WITH_ERRORS/modelization.json`

 * *Files identical despite different names*

### Comparing `cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/import_error_1y3_IMPORT_AT_CLUSTERING_STEP_WITH_ERRORS/settings.json` & `cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/import_error_1y3_IMPORT_AT_CLUSTERING_STEP_WITH_ERRORS/settings.json`

 * *Files identical despite different names*

### Comparing `cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/import_error_1y3_IMPORT_AT_CLUSTERING_STEP_WITH_ERRORS/texts.json` & `cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/import_error_1y3_IMPORT_AT_CLUSTERING_STEP_WITH_ERRORS/texts.json`

 * *Files identical despite different names*

### Comparing `cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/import_error_1y3_IMPORT_AT_CLUSTERING_STEP_WITH_ERRORS/vectors.pkl` & `cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/import_error_1y3_IMPORT_AT_CLUSTERING_STEP_WITH_ERRORS/vectors.pkl`

 * *Files identical despite different names*

### Comparing `cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/import_error_1y3_IMPORT_AT_CLUSTERING_STEP_WITH_ERRORS/vectors_2D.json` & `cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/import_error_1y3_IMPORT_AT_CLUSTERING_STEP_WITH_ERRORS/vectors_2D.json`

 * *Files identical despite different names*

### Comparing `cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/import_error_1y3_IMPORT_AT_CLUSTERING_STEP_WITH_ERRORS/vectors_3D.json` & `cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/import_error_1y3_IMPORT_AT_CLUSTERING_STEP_WITH_ERRORS/vectors_3D.json`

 * *Files identical despite different names*

### Comparing `cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/import_error_1z1_IMPORT_AT_ITERATION_END_WITH_PENDING_MODELIZATION/clustering.json` & `cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/import_error_1z1_IMPORT_AT_ITERATION_END_WITH_PENDING_MODELIZATION/clustering.json`

 * *Files identical despite different names*

### Comparing `cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/import_error_1z1_IMPORT_AT_ITERATION_END_WITH_PENDING_MODELIZATION/constraints.json` & `cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/import_error_1z1_IMPORT_AT_ITERATION_END_WITH_PENDING_MODELIZATION/constraints.json`

 * *Files identical despite different names*

### Comparing `cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/import_error_1z1_IMPORT_AT_ITERATION_END_WITH_PENDING_MODELIZATION/modelization.json` & `cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/import_error_1z1_IMPORT_AT_ITERATION_END_WITH_PENDING_MODELIZATION/modelization.json`

 * *Files identical despite different names*

### Comparing `cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/import_error_1z1_IMPORT_AT_ITERATION_END_WITH_PENDING_MODELIZATION/settings.json` & `cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/import_error_1z1_IMPORT_AT_ITERATION_END_WITH_PENDING_MODELIZATION/settings.json`

 * *Files identical despite different names*

### Comparing `cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/import_error_1z1_IMPORT_AT_ITERATION_END_WITH_PENDING_MODELIZATION/texts.json` & `cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/import_error_1z1_IMPORT_AT_ITERATION_END_WITH_PENDING_MODELIZATION/texts.json`

 * *Files identical despite different names*

### Comparing `cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/import_error_1z3_IMPORT_AT_ITERATION_END_WITH_ERRORS/clustering.json` & `cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/import_error_1z3_IMPORT_AT_ITERATION_END_WITH_ERRORS/clustering.json`

 * *Files identical despite different names*

### Comparing `cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/import_error_1z3_IMPORT_AT_ITERATION_END_WITH_ERRORS/constraints.json` & `cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/import_error_1z3_IMPORT_AT_ITERATION_END_WITH_ERRORS/constraints.json`

 * *Files identical despite different names*

### Comparing `cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/import_error_1z3_IMPORT_AT_ITERATION_END_WITH_ERRORS/constraints_manager.pkl` & `cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/import_error_1z3_IMPORT_AT_ITERATION_END_WITH_ERRORS/constraints_manager.pkl`

 * *Files identical despite different names*

### Comparing `cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/import_error_1z3_IMPORT_AT_ITERATION_END_WITH_ERRORS/modelization.json` & `cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/import_error_1z3_IMPORT_AT_ITERATION_END_WITH_ERRORS/modelization.json`

 * *Files identical despite different names*

### Comparing `cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/import_error_1z3_IMPORT_AT_ITERATION_END_WITH_ERRORS/settings.json` & `cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/import_error_1z3_IMPORT_AT_ITERATION_END_WITH_ERRORS/settings.json`

 * *Files identical despite different names*

### Comparing `cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/import_error_1z3_IMPORT_AT_ITERATION_END_WITH_ERRORS/texts.json` & `cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/import_error_1z3_IMPORT_AT_ITERATION_END_WITH_ERRORS/texts.json`

 * *Files identical despite different names*

### Comparing `cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/import_error_1z3_IMPORT_AT_ITERATION_END_WITH_ERRORS/vectors.pkl` & `cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/import_error_1z3_IMPORT_AT_ITERATION_END_WITH_ERRORS/vectors.pkl`

 * *Files identical despite different names*

### Comparing `cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/import_error_1z3_IMPORT_AT_ITERATION_END_WITH_ERRORS/vectors_2D.json` & `cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/import_error_1z3_IMPORT_AT_ITERATION_END_WITH_ERRORS/vectors_2D.json`

 * *Files identical despite different names*

### Comparing `cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies/import_error_1z3_IMPORT_AT_ITERATION_END_WITH_ERRORS/vectors_3D.json` & `cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies/import_error_1z3_IMPORT_AT_ITERATION_END_WITH_ERRORS/vectors_3D.json`

 * *Files identical despite different names*

### Comparing `cognitivefactory-interactive-clustering-gui-0.4.0/tests/dummies_utils.py` & `cognitivefactory-interactive-clustering-gui-0.4.1/tests/dummies_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -123,15 +123,14 @@
     """
 
     # Get path to dummy projects.
     path_to_dummy_projects: Path = Path(__file__).parent / "dummies"
 
     # For each request dummy project ID...
     for dummy_project_id in list_of_dummy_project_ids:
-
         # Copy the dummy project.
         if os.path.isdir(path_to_dummy_projects / dummy_project_id):
             shutil.copytree(
                 src=(path_to_dummy_projects / dummy_project_id),
                 dst=(tmp_path / dummy_project_id),
             )
         else:
```

### Comparing `cognitivefactory-interactive-clustering-gui-0.4.0/tests/test_app.py` & `cognitivefactory-interactive-clustering-gui-0.4.1/tests/test_app.py`

 * *Files identical despite different names*

### Comparing `cognitivefactory-interactive-clustering-gui-0.4.0/tests/test_backgroundtasks.py` & `cognitivefactory-interactive-clustering-gui-0.4.1/tests/test_backgroundtasks.py`

 * *Files identical despite different names*

### Comparing `cognitivefactory-interactive-clustering-gui-0.4.0/tests/test_cli.py` & `cognitivefactory-interactive-clustering-gui-0.4.1/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `cognitivefactory-interactive-clustering-gui-0.4.0/tests/test_delete_api_projects.py` & `cognitivefactory-interactive-clustering-gui-0.4.1/tests/test_delete_api_projects.py`

 * *Files identical despite different names*

### Comparing `cognitivefactory-interactive-clustering-gui-0.4.0/tests/test_get_alive.py` & `cognitivefactory-interactive-clustering-gui-0.4.1/tests/test_get_alive.py`

 * *Files identical despite different names*

### Comparing `cognitivefactory-interactive-clustering-gui-0.4.0/tests/test_get_api_projects.py` & `cognitivefactory-interactive-clustering-gui-0.4.1/tests/test_get_api_projects.py`

 * *Files identical despite different names*

### Comparing `cognitivefactory-interactive-clustering-gui-0.4.0/tests/test_get_api_projects_clustering.py` & `cognitivefactory-interactive-clustering-gui-0.4.1/tests/test_get_api_projects_clustering.py`

 * *Files identical despite different names*

### Comparing `cognitivefactory-interactive-clustering-gui-0.4.0/tests/test_get_api_projects_constraints.py` & `cognitivefactory-interactive-clustering-gui-0.4.1/tests/test_get_api_projects_constraints.py`

 * *Files identical despite different names*

### Comparing `cognitivefactory-interactive-clustering-gui-0.4.0/tests/test_get_api_projects_download.py` & `cognitivefactory-interactive-clustering-gui-0.4.1/tests/test_get_api_projects_download.py`

 * *Files identical despite different names*

### Comparing `cognitivefactory-interactive-clustering-gui-0.4.0/tests/test_get_api_projects_metadata.py` & `cognitivefactory-interactive-clustering-gui-0.4.1/tests/test_get_api_projects_metadata.py`

 * *Files identical despite different names*

### Comparing `cognitivefactory-interactive-clustering-gui-0.4.0/tests/test_get_api_projects_modelization.py` & `cognitivefactory-interactive-clustering-gui-0.4.1/tests/test_get_api_projects_modelization.py`

 * *Files identical despite different names*

### Comparing `cognitivefactory-interactive-clustering-gui-0.4.0/tests/test_get_api_projects_sampling.py` & `cognitivefactory-interactive-clustering-gui-0.4.1/tests/test_get_api_projects_sampling.py`

 * *Files identical despite different names*

### Comparing `cognitivefactory-interactive-clustering-gui-0.4.0/tests/test_get_api_projects_settings.py` & `cognitivefactory-interactive-clustering-gui-0.4.1/tests/test_get_api_projects_settings.py`

 * *Files identical despite different names*

### Comparing `cognitivefactory-interactive-clustering-gui-0.4.0/tests/test_get_api_projects_status.py` & `cognitivefactory-interactive-clustering-gui-0.4.1/tests/test_get_api_projects_status.py`

 * *Files identical despite different names*

### Comparing `cognitivefactory-interactive-clustering-gui-0.4.0/tests/test_get_api_projects_texts.py` & `cognitivefactory-interactive-clustering-gui-0.4.1/tests/test_get_api_projects_texts.py`

 * *Files identical despite different names*

### Comparing `cognitivefactory-interactive-clustering-gui-0.4.0/tests/test_get_api_projects_vectors.py` & `cognitivefactory-interactive-clustering-gui-0.4.1/tests/test_get_api_projects_vectors.py`

 * *Files identical despite different names*

### Comparing `cognitivefactory-interactive-clustering-gui-0.4.0/tests/test_get_gui_help.py` & `cognitivefactory-interactive-clustering-gui-0.4.1/tests/test_get_gui_help.py`

 * *Files identical despite different names*

### Comparing `cognitivefactory-interactive-clustering-gui-0.4.0/tests/test_get_gui_projects_constraints.py` & `cognitivefactory-interactive-clustering-gui-0.4.1/tests/test_get_gui_projects_constraints.py`

 * *Files identical despite different names*

### Comparing `cognitivefactory-interactive-clustering-gui-0.4.0/tests/test_get_gui_projects_constraints_annotation.py` & `cognitivefactory-interactive-clustering-gui-0.4.1/tests/test_get_gui_projects_constraints_annotation.py`

 * *Files identical despite different names*

### Comparing `cognitivefactory-interactive-clustering-gui-0.4.0/tests/test_get_gui_projects_home.py` & `cognitivefactory-interactive-clustering-gui-0.4.1/tests/test_get_gui_projects_home.py`

 * *Files identical despite different names*

### Comparing `cognitivefactory-interactive-clustering-gui-0.4.0/tests/test_get_gui_projects_listing.py` & `cognitivefactory-interactive-clustering-gui-0.4.1/tests/test_get_gui_projects_listing.py`

 * *Files identical despite different names*

### Comparing `cognitivefactory-interactive-clustering-gui-0.4.0/tests/test_get_gui_projects_settings.py` & `cognitivefactory-interactive-clustering-gui-0.4.1/tests/test_get_gui_projects_settings.py`

 * *Files identical despite different names*

### Comparing `cognitivefactory-interactive-clustering-gui-0.4.0/tests/test_get_gui_projects_texts.py` & `cognitivefactory-interactive-clustering-gui-0.4.1/tests/test_get_gui_projects_texts.py`

 * *Files identical despite different names*

### Comparing `cognitivefactory-interactive-clustering-gui-0.4.0/tests/test_get_ready.py` & `cognitivefactory-interactive-clustering-gui-0.4.1/tests/test_get_ready.py`

 * *Files identical despite different names*

### Comparing `cognitivefactory-interactive-clustering-gui-0.4.0/tests/test_get_welcome.py` & `cognitivefactory-interactive-clustering-gui-0.4.1/tests/test_get_welcome.py`

 * *Files identical despite different names*

### Comparing `cognitivefactory-interactive-clustering-gui-0.4.0/tests/test_post_api_projects.py` & `cognitivefactory-interactive-clustering-gui-0.4.1/tests/test_post_api_projects.py`

 * *Files identical despite different names*

### Comparing `cognitivefactory-interactive-clustering-gui-0.4.0/tests/test_post_api_projects_clustering.py` & `cognitivefactory-interactive-clustering-gui-0.4.1/tests/test_post_api_projects_clustering.py`

 * *Files identical despite different names*

### Comparing `cognitivefactory-interactive-clustering-gui-0.4.0/tests/test_post_api_projects_constraints_approve.py` & `cognitivefactory-interactive-clustering-gui-0.4.1/tests/test_post_api_projects_constraints_approve.py`

 * *Files identical despite different names*

### Comparing `cognitivefactory-interactive-clustering-gui-0.4.0/tests/test_post_api_projects_iterations.py` & `cognitivefactory-interactive-clustering-gui-0.4.1/tests/test_post_api_projects_iterations.py`

 * *Files identical despite different names*

### Comparing `cognitivefactory-interactive-clustering-gui-0.4.0/tests/test_post_api_projects_modelization.py` & `cognitivefactory-interactive-clustering-gui-0.4.1/tests/test_post_api_projects_modelization.py`

 * *Files identical despite different names*

### Comparing `cognitivefactory-interactive-clustering-gui-0.4.0/tests/test_post_api_projects_sampling.py` & `cognitivefactory-interactive-clustering-gui-0.4.1/tests/test_post_api_projects_sampling.py`

 * *Files identical despite different names*

### Comparing `cognitivefactory-interactive-clustering-gui-0.4.0/tests/test_put_api_projects.py` & `cognitivefactory-interactive-clustering-gui-0.4.1/tests/test_put_api_projects.py`

 * *Files identical despite different names*

### Comparing `cognitivefactory-interactive-clustering-gui-0.4.0/tests/test_put_api_projects_constraints_annotate.py` & `cognitivefactory-interactive-clustering-gui-0.4.1/tests/test_put_api_projects_constraints_annotate.py`

 * *Files identical despite different names*

### Comparing `cognitivefactory-interactive-clustering-gui-0.4.0/tests/test_put_api_projects_constraints_comment.py` & `cognitivefactory-interactive-clustering-gui-0.4.1/tests/test_put_api_projects_constraints_comment.py`

 * *Files identical despite different names*

### Comparing `cognitivefactory-interactive-clustering-gui-0.4.0/tests/test_put_api_projects_constraints_review.py` & `cognitivefactory-interactive-clustering-gui-0.4.1/tests/test_put_api_projects_constraints_review.py`

 * *Files identical despite different names*

### Comparing `cognitivefactory-interactive-clustering-gui-0.4.0/tests/test_put_api_projects_settings.py` & `cognitivefactory-interactive-clustering-gui-0.4.1/tests/test_put_api_projects_settings.py`

 * *Files identical despite different names*

### Comparing `cognitivefactory-interactive-clustering-gui-0.4.0/tests/test_put_api_projects_texts_delete.py` & `cognitivefactory-interactive-clustering-gui-0.4.1/tests/test_put_api_projects_texts_delete.py`

 * *Files identical despite different names*

### Comparing `cognitivefactory-interactive-clustering-gui-0.4.0/tests/test_put_api_projects_texts_rename.py` & `cognitivefactory-interactive-clustering-gui-0.4.1/tests/test_put_api_projects_texts_rename.py`

 * *Files identical despite different names*

### Comparing `cognitivefactory-interactive-clustering-gui-0.4.0/tests/test_put_api_projects_texts_undelete.py` & `cognitivefactory-interactive-clustering-gui-0.4.1/tests/test_put_api_projects_texts_undelete.py`

 * *Files identical despite different names*

### Comparing `cognitivefactory-interactive-clustering-gui-0.4.0/tests/test_run_constrained_clustering_task.py` & `cognitivefactory-interactive-clustering-gui-0.4.1/tests/test_run_constrained_clustering_task.py`

 * *Files identical despite different names*

### Comparing `cognitivefactory-interactive-clustering-gui-0.4.0/tests/test_run_constraints_sampling_task.py` & `cognitivefactory-interactive-clustering-gui-0.4.1/tests/test_run_constraints_sampling_task.py`

 * *Files identical despite different names*

### Comparing `cognitivefactory-interactive-clustering-gui-0.4.0/tests/test_run_modelization_update_task.py` & `cognitivefactory-interactive-clustering-gui-0.4.1/tests/test_run_modelization_update_task.py`

 * *Files identical despite different names*

### Comparing `cognitivefactory-interactive-clustering-gui-0.4.0/tests/test_utils_jinja_filters.py` & `cognitivefactory-interactive-clustering-gui-0.4.1/tests/test_utils_jinja_filters.py`

 * *Files identical despite different names*

### Comparing `cognitivefactory-interactive-clustering-gui-0.4.0/tests/test_utils_models_settings.py` & `cognitivefactory-interactive-clustering-gui-0.4.1/tests/test_utils_models_settings.py`

 * *Files identical despite different names*

### Comparing `cognitivefactory-interactive-clustering-gui-0.4.0/tests/test_utils_models_states.py` & `cognitivefactory-interactive-clustering-gui-0.4.1/tests/test_utils_models_states.py`

 * *Files identical despite different names*

