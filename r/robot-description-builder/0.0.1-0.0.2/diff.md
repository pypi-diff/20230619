# Comparing `tmp/robot_description_builder-0.0.1.tar.gz` & `tmp/robot_description_builder-0.0.2.tar.gz`

## Comparing `robot_description_builder-0.0.1.tar` & `robot_description_builder-0.0.2.tar`

### file list

```diff
@@ -1,104 +1,149 @@
--rw-r--r--   0        0        0      635 1970-01-01 00:00:00.000000 robot_description_builder-0.0.1/local_dependencies/robot-description-builder/Cargo.toml
--rw-r--r--   0     1000     1000     1073 2023-05-09 18:35:16.000000 robot_description_builder-0.0.1/local_dependencies/robot-description-builder/LICENSE
--rw-r--r--   0     1000     1000      135 2023-05-09 18:39:30.000000 robot_description_builder-0.0.1/local_dependencies/robot-description-builder/README.md
--rw-r--r--   0     1000     1000     2299 2023-05-08 18:37:03.000000 robot_description_builder-0.0.1/local_dependencies/robot-description-builder/examples/example-1.rs
--rw-r--r--   0     1000     1000     1546 2023-05-08 18:36:46.000000 robot_description_builder-0.0.1/local_dependencies/robot-description-builder/examples/smart_builder_example.rs
--rw-r--r--   0     1000     1000      792 2023-05-08 18:36:43.000000 robot_description_builder-0.0.1/local_dependencies/robot-description-builder/examples/transmission-example.rs
--rw-r--r--   0     1000     1000     1273 2023-05-08 18:36:40.000000 robot_description_builder-0.0.1/local_dependencies/robot-description-builder/examples/urdf-tutorial-02.rs
--rw-r--r--   0     1000     1000     4434 2023-05-08 18:38:59.000000 robot_description_builder-0.0.1/local_dependencies/robot-description-builder/examples/urdf-tutorial-05-visual.rs
--rw-r--r--   0     1000     1000     4729 2023-05-08 18:36:16.000000 robot_description_builder-0.0.1/local_dependencies/robot-description-builder/examples/urdf-tutorial-06-flexible.rs
--rw-r--r--   0     1000     1000    10444 2023-05-08 13:01:55.000000 robot_description_builder-0.0.1/local_dependencies/robot-description-builder/src/chained/chained_jointbuilder.rs
--rw-r--r--   0     1000     1000     9232 2023-05-08 13:05:45.000000 robot_description_builder-0.0.1/local_dependencies/robot-description-builder/src/chained/chained_linkbuilder.rs
--rw-r--r--   0     1000     1000     5192 2023-05-03 11:51:50.000000 robot_description_builder-0.0.1/local_dependencies/robot-description-builder/src/chained/mod.rs
--rw-r--r--   0     1000     1000     7915 2023-05-04 14:30:49.000000 robot_description_builder-0.0.1/local_dependencies/robot-description-builder/src/cluster_objects/kinematic_data_errors.rs
--rw-r--r--   0     1000     1000    21775 2023-05-05 14:27:27.000000 robot_description_builder-0.0.1/local_dependencies/robot-description-builder/src/cluster_objects/kinematic_data_tree.rs
--rw-r--r--   0     1000     1000    16750 2023-05-08 18:33:13.000000 robot_description_builder-0.0.1/local_dependencies/robot-description-builder/src/cluster_objects/kinematic_tree.rs
--rw-r--r--   0     1000     1000     4179 2023-05-08 18:31:27.000000 robot_description_builder-0.0.1/local_dependencies/robot-description-builder/src/cluster_objects/robot.rs
--rw-r--r--   0     1000     1000     5308 2023-05-08 18:40:37.000000 robot_description_builder-0.0.1/local_dependencies/robot-description-builder/src/cluster_objects.rs
--rw-r--r--   0     1000     1000    24637 2023-05-08 19:01:46.000000 robot_description_builder-0.0.1/local_dependencies/robot-description-builder/src/identifiers.rs
--rw-r--r--   0     1000     1000     4997 2023-05-08 18:39:03.000000 robot_description_builder-0.0.1/local_dependencies/robot-description-builder/src/joint/joint_data/calibration_data.rs
--rw-r--r--   0     1000     1000     4809 2023-05-08 18:31:19.000000 robot_description_builder-0.0.1/local_dependencies/robot-description-builder/src/joint/joint_data/dynamics_data.rs
--rw-r--r--   0     1000     1000     4906 2023-04-30 17:19:15.000000 robot_description_builder-0.0.1/local_dependencies/robot-description-builder/src/joint/joint_data/limit_data.rs
--rw-r--r--   0     1000     1000     6289 2023-05-05 13:25:04.000000 robot_description_builder-0.0.1/local_dependencies/robot-description-builder/src/joint/joint_data/mimic_data.rs
--rw-r--r--   0     1000     1000     7656 2023-04-30 17:19:15.000000 robot_description_builder-0.0.1/local_dependencies/robot-description-builder/src/joint/joint_data/safety_controller_data.rs
--rw-r--r--   0     1000     1000      318 2023-04-30 17:19:15.000000 robot_description_builder-0.0.1/local_dependencies/robot-description-builder/src/joint/joint_data.rs
--rw-r--r--   0     1000     1000     1792 2023-05-08 13:05:52.000000 robot_description_builder-0.0.1/local_dependencies/robot-description-builder/src/joint/joint_tranform_mode.rs
--rw-r--r--   0     1000     1000    10707 2023-05-08 13:03:15.000000 robot_description_builder-0.0.1/local_dependencies/robot-description-builder/src/joint/jointbuilder.rs
--rw-r--r--   0     1000     1000     2922 2023-05-03 09:18:40.000000 robot_description_builder-0.0.1/local_dependencies/robot-description-builder/src/joint/smartjointbuilder/smartjointtypes/continuous_joint_type.rs
--rw-r--r--   0     1000     1000     1453 2023-05-03 09:18:35.000000 robot_description_builder-0.0.1/local_dependencies/robot-description-builder/src/joint/smartjointbuilder/smartjointtypes/fixed_joint_type.rs
--rw-r--r--   0     1000     1000     4575 2023-05-03 09:18:28.000000 robot_description_builder-0.0.1/local_dependencies/robot-description-builder/src/joint/smartjointbuilder/smartjointtypes/floating_joint_type.rs
--rw-r--r--   0     1000     1000     3019 2023-05-03 09:18:19.000000 robot_description_builder-0.0.1/local_dependencies/robot-description-builder/src/joint/smartjointbuilder/smartjointtypes/planar_joint_type.rs
--rw-r--r--   0     1000     1000     2849 2023-05-03 09:18:53.000000 robot_description_builder-0.0.1/local_dependencies/robot-description-builder/src/joint/smartjointbuilder/smartjointtypes/prismatic_joint_type.rs
--rw-r--r--   0     1000     1000     2807 2023-05-03 09:19:01.000000 robot_description_builder-0.0.1/local_dependencies/robot-description-builder/src/joint/smartjointbuilder/smartjointtypes/revolute_joint_type.rs
--rw-r--r--   0     1000     1000      477 2023-05-03 09:19:11.000000 robot_description_builder-0.0.1/local_dependencies/robot-description-builder/src/joint/smartjointbuilder/smartjointtypes.rs
--rw-r--r--   0     1000     1000     1774 2023-04-30 17:19:15.000000 robot_description_builder-0.0.1/local_dependencies/robot-description-builder/src/joint/smartjointbuilder/smartparams/axis.rs
--rw-r--r--   0     1000     1000     2320 2023-04-30 17:19:15.000000 robot_description_builder-0.0.1/local_dependencies/robot-description-builder/src/joint/smartjointbuilder/smartparams/calibration.rs
--rw-r--r--   0     1000     1000     2280 2023-04-30 17:19:15.000000 robot_description_builder-0.0.1/local_dependencies/robot-description-builder/src/joint/smartjointbuilder/smartparams/dynamics.rs
--rw-r--r--   0     1000     1000     3495 2023-04-30 17:19:15.000000 robot_description_builder-0.0.1/local_dependencies/robot-description-builder/src/joint/smartjointbuilder/smartparams/limit.rs
--rw-r--r--   0     1000     1000     3219 2023-04-30 17:19:15.000000 robot_description_builder-0.0.1/local_dependencies/robot-description-builder/src/joint/smartjointbuilder/smartparams/mimic.rs
--rw-r--r--   0     1000     1000     3840 2023-04-30 17:19:15.000000 robot_description_builder-0.0.1/local_dependencies/robot-description-builder/src/joint/smartjointbuilder/smartparams/safety_controller.rs
--rw-r--r--   0     1000     1000     1458 2023-04-30 17:19:15.000000 robot_description_builder-0.0.1/local_dependencies/robot-description-builder/src/joint/smartjointbuilder/smartparams.rs
--rw-r--r--   0     1000     1000     6313 2023-05-03 09:22:32.000000 robot_description_builder-0.0.1/local_dependencies/robot-description-builder/src/joint/smartjointbuilder.rs
--rw-r--r--   0     1000     1000    20736 2023-05-05 14:35:34.000000 robot_description_builder-0.0.1/local_dependencies/robot-description-builder/src/joint.rs
--rw-r--r--   0     1000     1000      984 2023-05-05 13:17:09.000000 robot_description_builder-0.0.1/local_dependencies/robot-description-builder/src/lib.rs
--rw-r--r--   0     1000     1000    11075 2023-05-08 15:40:48.000000 robot_description_builder-0.0.1/local_dependencies/robot-description-builder/src/link/builder/collision_builder.rs
--rw-r--r--   0     1000     1000    10971 2023-05-08 13:08:24.000000 robot_description_builder-0.0.1/local_dependencies/robot-description-builder/src/link/builder/linkbuilder.rs
--rw-r--r--   0     1000     1000    12176 2023-05-08 15:45:58.000000 robot_description_builder-0.0.1/local_dependencies/robot-description-builder/src/link/builder/visual_builder.rs
--rw-r--r--   0     1000     1000     1367 2023-05-03 11:31:36.000000 robot_description_builder-0.0.1/local_dependencies/robot-description-builder/src/link/builder.rs
--rw-r--r--   0     1000     1000     4279 2023-05-08 15:43:31.000000 robot_description_builder-0.0.1/local_dependencies/robot-description-builder/src/link/collision.rs
--rw-r--r--   0     1000     1000     6059 2023-05-08 15:40:48.000000 robot_description_builder-0.0.1/local_dependencies/robot-description-builder/src/link/geometry/box_geometry.rs
--rw-r--r--   0     1000     1000     6239 2023-05-08 15:40:48.000000 robot_description_builder-0.0.1/local_dependencies/robot-description-builder/src/link/geometry/cylinder_geometry.rs
--rw-r--r--   0     1000     1000     2125 2023-05-08 13:39:28.000000 robot_description_builder-0.0.1/local_dependencies/robot-description-builder/src/link/geometry/geometry_shape_data.rs
--rw-r--r--   0     1000     1000    10976 2023-05-08 15:40:48.000000 robot_description_builder-0.0.1/local_dependencies/robot-description-builder/src/link/geometry/mesh_geometry.rs
--rw-r--r--   0     1000     1000     5803 2023-05-08 15:40:48.000000 robot_description_builder-0.0.1/local_dependencies/robot-description-builder/src/link/geometry/sphere_geometry.rs
--rw-r--r--   0     1000     1000     2121 2023-05-08 15:43:31.000000 robot_description_builder-0.0.1/local_dependencies/robot-description-builder/src/link/geometry.rs
--rw-r--r--   0     1000     1000     3347 2023-05-03 11:17:55.000000 robot_description_builder-0.0.1/local_dependencies/robot-description-builder/src/link/helper_functions.rs
--rw-r--r--   0     1000     1000     3292 2023-05-08 13:08:45.000000 robot_description_builder-0.0.1/local_dependencies/robot-description-builder/src/link/inertial.rs
--rw-r--r--   0     1000     1000     1028 2023-04-30 17:19:15.000000 robot_description_builder-0.0.1/local_dependencies/robot-description-builder/src/link/link_parent.rs
--rw-r--r--   0     1000     1000     1027 2023-05-03 11:27:45.000000 robot_description_builder-0.0.1/local_dependencies/robot-description-builder/src/link/link_shape_data.rs
--rw-r--r--   0     1000     1000     6496 2023-05-08 15:43:31.000000 robot_description_builder-0.0.1/local_dependencies/robot-description-builder/src/link/visual.rs
--rw-r--r--   0     1000     1000    14365 2023-05-08 18:40:40.000000 robot_description_builder-0.0.1/local_dependencies/robot-description-builder/src/link.rs
--rw-r--r--   0     1000     1000     5145 2023-05-04 15:32:45.000000 robot_description_builder-0.0.1/local_dependencies/robot-description-builder/src/material/data.rs
--rw-r--r--   0     1000     1000    15662 2023-05-08 18:31:15.000000 robot_description_builder-0.0.1/local_dependencies/robot-description-builder/src/material/descriptor.rs
--rw-r--r--   0     1000     1000     2708 2023-05-04 15:05:52.000000 robot_description_builder-0.0.1/local_dependencies/robot-description-builder/src/material/stage.rs
--rw-r--r--   0     1000     1000     9602 2023-05-04 16:27:56.000000 robot_description_builder-0.0.1/local_dependencies/robot-description-builder/src/material.rs
--rw-r--r--   0     1000     1000     1053 2023-05-03 11:02:09.000000 robot_description_builder-0.0.1/local_dependencies/robot-description-builder/src/to_rdf/to_sdf.rs
--rw-r--r--   0     1000     1000     2264 2023-05-05 14:17:02.000000 robot_description_builder-0.0.1/local_dependencies/robot-description-builder/src/to_rdf/to_urdf.rs
--rw-r--r--   0     1000     1000     1214 2023-05-04 15:34:24.000000 robot_description_builder-0.0.1/local_dependencies/robot-description-builder/src/to_rdf.rs
--rw-r--r--   0     1000     1000    16861 2023-05-08 18:40:42.000000 robot_description_builder-0.0.1/local_dependencies/robot-description-builder/src/transform.rs
--rw-r--r--   0     1000     1000      652 2023-05-02 17:39:05.000000 robot_description_builder-0.0.1/local_dependencies/robot-description-builder/src/transmission/build_transmission_error.rs
--rw-r--r--   0     1000     1000     5152 2023-05-02 20:11:30.000000 robot_description_builder-0.0.1/local_dependencies/robot-description-builder/src/transmission/hardware_interface.rs
--rw-r--r--   0     1000     1000    17682 2023-05-04 16:27:32.000000 robot_description_builder-0.0.1/local_dependencies/robot-description-builder/src/transmission/mod.rs
--rw-r--r--   0     1000     1000     1955 2023-05-04 16:27:43.000000 robot_description_builder-0.0.1/local_dependencies/robot-description-builder/src/transmission/transmission_actuator.rs
--rw-r--r--   0     1000     1000     4514 2023-05-04 16:27:58.000000 robot_description_builder-0.0.1/local_dependencies/robot-description-builder/src/transmission/transmission_joint.rs
--rw-r--r--   0     1000     1000     1771 2023-05-02 20:11:30.000000 robot_description_builder-0.0.1/local_dependencies/robot-description-builder/src/transmission/transmission_type.rs
--rw-r--r--   0        0        0      402 1970-01-01 00:00:00.000000 robot_description_builder-0.0.1/Cargo.toml
--rw-r--r--   0     1000     1000      686 2023-04-30 17:19:15.000000 robot_description_builder-0.0.1/.gitignore
--rw-r--r--   0     1000     1000     1073 2023-05-09 18:35:07.000000 robot_description_builder-0.0.1/LICENSE
--rw-r--r--   0     1000     1000      294 2023-05-09 18:52:58.000000 robot_description_builder-0.0.1/README.md
--rwxr-xr-x   0     1000     1000      218 2023-05-09 11:45:22.000000 robot_description_builder-0.0.1/examples/urdf-tutorial-05-visual.py
--rw-r--r--   0     1000     1000      622 2023-05-09 18:29:35.000000 robot_description_builder-0.0.1/pyproject.toml
--rw-r--r--   0     1000     1000      578 2023-05-09 12:24:24.000000 robot_description_builder-0.0.1/python/robot_description_builder/__init__.py
--rw-r--r--   0     1000     1000      225 2023-05-09 13:21:15.000000 robot_description_builder-0.0.1/python/robot_description_builder/link/__init__.py
--rw-r--r--   0     1000     1000       52 2023-05-09 13:10:27.000000 robot_description_builder-0.0.1/python/robot_description_builder/link/collision.py
--rw-r--r--   0     1000     1000      111 2023-05-09 12:40:58.000000 robot_description_builder-0.0.1/python/robot_description_builder/link/geometry.py
--rw-r--r--   0     1000     1000       46 2023-05-09 12:42:24.000000 robot_description_builder-0.0.1/python/robot_description_builder/link/visual.py
--rw-r--r--   0     1000     1000     1325 2023-05-03 15:57:12.000000 robot_description_builder-0.0.1/rdf_builder_py.pyi.old
--rw-r--r--   0     1000     1000       14 2023-04-30 17:19:15.000000 robot_description_builder-0.0.1/requirements-dev.txt
--rw-r--r--   0     1000     1000     3192 2023-05-08 18:38:12.000000 robot_description_builder-0.0.1/src/joint.rs
--rw-r--r--   0     1000     1000     4589 2023-05-09 12:44:11.000000 robot_description_builder-0.0.1/src/lib.rs
--rw-r--r--   0     1000     1000     2083 2023-05-09 12:44:11.000000 robot_description_builder-0.0.1/src/link/collision.rs
--rw-r--r--   0     1000     1000     1732 2023-05-09 12:52:46.000000 robot_description_builder-0.0.1/src/link/geometry/box_geometry.rs
--rw-r--r--   0     1000     1000     2294 2023-05-09 12:53:49.000000 robot_description_builder-0.0.1/src/link/geometry/cylinder_geometry.rs
--rw-r--r--   0     1000     1000     1503 2023-05-09 12:54:08.000000 robot_description_builder-0.0.1/src/link/geometry/sphere_geometry.rs
--rw-r--r--   0     1000     1000     1851 2023-05-09 12:46:47.000000 robot_description_builder-0.0.1/src/link/geometry.rs
--rw-r--r--   0     1000     1000     2978 2023-05-09 12:56:39.000000 robot_description_builder-0.0.1/src/link/inertial.rs
--rw-r--r--   0     1000     1000     3122 2023-05-09 12:58:29.000000 robot_description_builder-0.0.1/src/link/visual.rs
--rw-r--r--   0     1000     1000     5895 2023-05-09 13:06:49.000000 robot_description_builder-0.0.1/src/link.rs
--rw-r--r--   0     1000     1000     1430 2023-05-08 18:37:52.000000 robot_description_builder-0.0.1/src/material.rs
--rw-r--r--   0     1000     1000     5132 2023-05-09 12:59:00.000000 robot_description_builder-0.0.1/src/material_descriptor.rs
--rw-r--r--   0     1000     1000     3653 2023-05-08 18:37:39.000000 robot_description_builder-0.0.1/src/transform.rs
--rw-r--r--   0     1000     1000     1151 2023-05-03 20:11:59.000000 robot_description_builder-0.0.1/src/utils.rs
--rw-r--r--   0     1000     1000      609 2023-05-09 18:18:39.000000 robot_description_builder-0.0.1/tests/test_link.py
--rw-r--r--   0     1000     1000    19843 2023-05-09 18:29:26.000000 robot_description_builder-0.0.1/Cargo.lock
--rw-r--r--   0        0        0      673 1970-01-01 00:00:00.000000 robot_description_builder-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0      307 1970-01-01 00:00:00.000000 robot_description_builder-0.0.2/local_dependencies/rdb-py-macro/Cargo.toml
+-rw-r--r--   0     1001      123    11819 2023-06-19 00:27:33.000000 robot_description_builder-0.0.2/local_dependencies/rdb-py-macro/src/code_gen.rs
+-rw-r--r--   0     1001      123     1219 2023-06-19 00:27:33.000000 robot_description_builder-0.0.2/local_dependencies/rdb-py-macro/src/conversion_impls.rs
+-rw-r--r--   0     1001      123     1631 2023-06-19 00:27:33.000000 robot_description_builder-0.0.2/local_dependencies/rdb-py-macro/src/enum_generation.rs
+-rw-r--r--   0     1001      123      978 2023-06-19 00:27:33.000000 robot_description_builder-0.0.2/local_dependencies/rdb-py-macro/src/error_gen.rs
+-rw-r--r--   0     1001      123     2054 2023-06-19 00:27:33.000000 robot_description_builder-0.0.2/local_dependencies/rdb-py-macro/src/lib.rs
+-rw-r--r--   0     1001      123     2517 2023-06-19 00:27:33.000000 robot_description_builder-0.0.2/local_dependencies/rdb-py-macro/src/parse.rs
+-rw-r--r--   0        0        0      905 1970-01-01 00:00:00.000000 robot_description_builder-0.0.2/local_dependencies/robot-description-builder/Cargo.toml
+-rw-r--r--   0     1001      123     1073 2023-06-19 00:27:33.000000 robot_description_builder-0.0.2/local_dependencies/robot-description-builder/LICENSE
+-rw-r--r--   0     1001      123     3952 2023-06-19 00:27:33.000000 robot_description_builder-0.0.2/local_dependencies/robot-description-builder/README.md
+-rw-r--r--   0     1001      123     2299 2023-06-19 00:27:33.000000 robot_description_builder-0.0.2/local_dependencies/robot-description-builder/examples/example-1.rs
+-rw-r--r--   0     1001      123     1546 2023-06-19 00:27:33.000000 robot_description_builder-0.0.2/local_dependencies/robot-description-builder/examples/smart_builder_example.rs
+-rw-r--r--   0     1001      123      792 2023-06-19 00:27:33.000000 robot_description_builder-0.0.2/local_dependencies/robot-description-builder/examples/transmission-example.rs
+-rw-r--r--   0     1001      123     1273 2023-06-19 00:27:33.000000 robot_description_builder-0.0.2/local_dependencies/robot-description-builder/examples/urdf-tutorial-02.rs
+-rw-r--r--   0     1001      123     6593 2023-06-19 00:27:33.000000 robot_description_builder-0.0.2/local_dependencies/robot-description-builder/examples/urdf-tutorial-05-visual.rs
+-rw-r--r--   0     1001      123     7086 2023-06-19 00:27:33.000000 robot_description_builder-0.0.2/local_dependencies/robot-description-builder/examples/urdf-tutorial-06-flexible.rs
+-rw-r--r--   0     1001      123    10928 2023-06-19 00:27:33.000000 robot_description_builder-0.0.2/local_dependencies/robot-description-builder/src/chained/chained_jointbuilder.rs
+-rw-r--r--   0     1001      123     9167 2023-06-19 00:27:33.000000 robot_description_builder-0.0.2/local_dependencies/robot-description-builder/src/chained/chained_linkbuilder.rs
+-rw-r--r--   0     1001      123     5718 2023-06-19 00:27:33.000000 robot_description_builder-0.0.2/local_dependencies/robot-description-builder/src/chained/mod.rs
+-rw-r--r--   0     1001      123     7915 2023-06-19 00:27:33.000000 robot_description_builder-0.0.2/local_dependencies/robot-description-builder/src/cluster_objects/kinematic_data_errors.rs
+-rw-r--r--   0     1001      123    21818 2023-06-19 00:27:33.000000 robot_description_builder-0.0.2/local_dependencies/robot-description-builder/src/cluster_objects/kinematic_data_tree.rs
+-rw-r--r--   0     1001      123    16646 2023-06-19 00:27:33.000000 robot_description_builder-0.0.2/local_dependencies/robot-description-builder/src/cluster_objects/kinematic_tree.rs
+-rw-r--r--   0     1001      123     4078 2023-06-19 00:27:33.000000 robot_description_builder-0.0.2/local_dependencies/robot-description-builder/src/cluster_objects/robot.rs
+-rw-r--r--   0     1001      123     5972 2023-06-19 00:27:33.000000 robot_description_builder-0.0.2/local_dependencies/robot-description-builder/src/cluster_objects.rs
+-rw-r--r--   0     1001      123    24637 2023-06-19 00:27:33.000000 robot_description_builder-0.0.2/local_dependencies/robot-description-builder/src/identifiers.rs
+-rw-r--r--   0     1001      123     4978 2023-06-19 00:27:33.000000 robot_description_builder-0.0.2/local_dependencies/robot-description-builder/src/joint/joint_data/calibration_data.rs
+-rw-r--r--   0     1001      123     4809 2023-06-19 00:27:33.000000 robot_description_builder-0.0.2/local_dependencies/robot-description-builder/src/joint/joint_data/dynamics_data.rs
+-rw-r--r--   0     1001      123     4906 2023-06-19 00:27:33.000000 robot_description_builder-0.0.2/local_dependencies/robot-description-builder/src/joint/joint_data/limit_data.rs
+-rw-r--r--   0     1001      123     6289 2023-06-19 00:27:33.000000 robot_description_builder-0.0.2/local_dependencies/robot-description-builder/src/joint/joint_data/mimic_data.rs
+-rw-r--r--   0     1001      123     7656 2023-06-19 00:27:33.000000 robot_description_builder-0.0.2/local_dependencies/robot-description-builder/src/joint/joint_data/safety_controller_data.rs
+-rw-r--r--   0     1001      123      318 2023-06-19 00:27:33.000000 robot_description_builder-0.0.2/local_dependencies/robot-description-builder/src/joint/joint_data.rs
+-rw-r--r--   0     1001      123     1792 2023-06-19 00:27:33.000000 robot_description_builder-0.0.2/local_dependencies/robot-description-builder/src/joint/joint_tranform_mode.rs
+-rw-r--r--   0     1001      123    13052 2023-06-19 00:27:33.000000 robot_description_builder-0.0.2/local_dependencies/robot-description-builder/src/joint/jointbuilder.rs
+-rw-r--r--   0     1001      123     3036 2023-06-19 00:27:33.000000 robot_description_builder-0.0.2/local_dependencies/robot-description-builder/src/joint/smartjointbuilder/smartjointtypes/continuous_joint_type.rs
+-rw-r--r--   0     1001      123     1496 2023-06-19 00:27:33.000000 robot_description_builder-0.0.2/local_dependencies/robot-description-builder/src/joint/smartjointbuilder/smartjointtypes/fixed_joint_type.rs
+-rw-r--r--   0     1001      123     4650 2023-06-19 00:27:33.000000 robot_description_builder-0.0.2/local_dependencies/robot-description-builder/src/joint/smartjointbuilder/smartjointtypes/floating_joint_type.rs
+-rw-r--r--   0     1001      123     3125 2023-06-19 00:27:33.000000 robot_description_builder-0.0.2/local_dependencies/robot-description-builder/src/joint/smartjointbuilder/smartjointtypes/planar_joint_type.rs
+-rw-r--r--   0     1001      123     2941 2023-06-19 00:27:33.000000 robot_description_builder-0.0.2/local_dependencies/robot-description-builder/src/joint/smartjointbuilder/smartjointtypes/prismatic_joint_type.rs
+-rw-r--r--   0     1001      123     2898 2023-06-19 00:27:33.000000 robot_description_builder-0.0.2/local_dependencies/robot-description-builder/src/joint/smartjointbuilder/smartjointtypes/revolute_joint_type.rs
+-rw-r--r--   0     1001      123     1025 2023-06-19 00:27:33.000000 robot_description_builder-0.0.2/local_dependencies/robot-description-builder/src/joint/smartjointbuilder/smartjointtypes.rs
+-rw-r--r--   0     1001      123     2105 2023-06-19 00:27:33.000000 robot_description_builder-0.0.2/local_dependencies/robot-description-builder/src/joint/smartjointbuilder/smartparams/axis.rs
+-rw-r--r--   0     1001      123     2484 2023-06-19 00:27:33.000000 robot_description_builder-0.0.2/local_dependencies/robot-description-builder/src/joint/smartjointbuilder/smartparams/calibration.rs
+-rw-r--r--   0     1001      123     2418 2023-06-19 00:27:33.000000 robot_description_builder-0.0.2/local_dependencies/robot-description-builder/src/joint/smartjointbuilder/smartparams/dynamics.rs
+-rw-r--r--   0     1001      123     4069 2023-06-19 00:27:33.000000 robot_description_builder-0.0.2/local_dependencies/robot-description-builder/src/joint/smartjointbuilder/smartparams/limit.rs
+-rw-r--r--   0     1001      123     3219 2023-06-19 00:27:33.000000 robot_description_builder-0.0.2/local_dependencies/robot-description-builder/src/joint/smartjointbuilder/smartparams/mimic.rs
+-rw-r--r--   0     1001      123     4286 2023-06-19 00:27:33.000000 robot_description_builder-0.0.2/local_dependencies/robot-description-builder/src/joint/smartjointbuilder/smartparams/safety_controller.rs
+-rw-r--r--   0     1001      123     1538 2023-06-19 00:27:33.000000 robot_description_builder-0.0.2/local_dependencies/robot-description-builder/src/joint/smartjointbuilder/smartparams.rs
+-rw-r--r--   0     1001      123     7746 2023-06-19 00:27:33.000000 robot_description_builder-0.0.2/local_dependencies/robot-description-builder/src/joint/smartjointbuilder.rs
+-rw-r--r--   0     1001      123    21342 2023-06-19 00:27:33.000000 robot_description_builder-0.0.2/local_dependencies/robot-description-builder/src/joint.rs
+-rw-r--r--   0     1001      123     1597 2023-06-19 00:27:33.000000 robot_description_builder-0.0.2/local_dependencies/robot-description-builder/src/lib.rs
+-rw-r--r--   0     1001      123    10968 2023-06-19 00:27:33.000000 robot_description_builder-0.0.2/local_dependencies/robot-description-builder/src/link/builder/collision_builder.rs
+-rw-r--r--   0     1001      123    10995 2023-06-19 00:27:33.000000 robot_description_builder-0.0.2/local_dependencies/robot-description-builder/src/link/builder/linkbuilder.rs
+-rw-r--r--   0     1001      123    12094 2023-06-19 00:27:33.000000 robot_description_builder-0.0.2/local_dependencies/robot-description-builder/src/link/builder/visual_builder.rs
+-rw-r--r--   0     1001      123     1367 2023-06-19 00:27:33.000000 robot_description_builder-0.0.2/local_dependencies/robot-description-builder/src/link/builder.rs
+-rw-r--r--   0     1001      123     4279 2023-06-19 00:27:33.000000 robot_description_builder-0.0.2/local_dependencies/robot-description-builder/src/link/collision.rs
+-rw-r--r--   0     1001      123     6059 2023-06-19 00:27:33.000000 robot_description_builder-0.0.2/local_dependencies/robot-description-builder/src/link/geometry/box_geometry.rs
+-rw-r--r--   0     1001      123     6239 2023-06-19 00:27:33.000000 robot_description_builder-0.0.2/local_dependencies/robot-description-builder/src/link/geometry/cylinder_geometry.rs
+-rw-r--r--   0     1001      123     2125 2023-06-19 00:27:33.000000 robot_description_builder-0.0.2/local_dependencies/robot-description-builder/src/link/geometry/geometry_shape_data.rs
+-rw-r--r--   0     1001      123    10976 2023-06-19 00:27:33.000000 robot_description_builder-0.0.2/local_dependencies/robot-description-builder/src/link/geometry/mesh_geometry.rs
+-rw-r--r--   0     1001      123     5803 2023-06-19 00:27:33.000000 robot_description_builder-0.0.2/local_dependencies/robot-description-builder/src/link/geometry/sphere_geometry.rs
+-rw-r--r--   0     1001      123     2202 2023-06-19 00:27:33.000000 robot_description_builder-0.0.2/local_dependencies/robot-description-builder/src/link/geometry.rs
+-rw-r--r--   0     1001      123     3347 2023-06-19 00:27:33.000000 robot_description_builder-0.0.2/local_dependencies/robot-description-builder/src/link/helper_functions.rs
+-rw-r--r--   0     1001      123     3291 2023-06-19 00:27:33.000000 robot_description_builder-0.0.2/local_dependencies/robot-description-builder/src/link/inertial.rs
+-rw-r--r--   0     1001      123     1028 2023-06-19 00:27:33.000000 robot_description_builder-0.0.2/local_dependencies/robot-description-builder/src/link/link_parent.rs
+-rw-r--r--   0     1001      123     1027 2023-06-19 00:27:33.000000 robot_description_builder-0.0.2/local_dependencies/robot-description-builder/src/link/link_shape_data.rs
+-rw-r--r--   0     1001      123     6484 2023-06-19 00:27:33.000000 robot_description_builder-0.0.2/local_dependencies/robot-description-builder/src/link/visual.rs
+-rw-r--r--   0     1001      123    14367 2023-06-19 00:27:33.000000 robot_description_builder-0.0.2/local_dependencies/robot-description-builder/src/link.rs
+-rw-r--r--   0     1001      123     5145 2023-06-19 00:27:33.000000 robot_description_builder-0.0.2/local_dependencies/robot-description-builder/src/material/data.rs
+-rw-r--r--   0     1001      123    15662 2023-06-19 00:27:33.000000 robot_description_builder-0.0.2/local_dependencies/robot-description-builder/src/material/descriptor.rs
+-rw-r--r--   0     1001      123     2732 2023-06-19 00:27:33.000000 robot_description_builder-0.0.2/local_dependencies/robot-description-builder/src/material/stage.rs
+-rw-r--r--   0     1001      123    10139 2023-06-19 00:27:33.000000 robot_description_builder-0.0.2/local_dependencies/robot-description-builder/src/material.rs
+-rw-r--r--   0     1001      123     1053 2023-06-19 00:27:33.000000 robot_description_builder-0.0.2/local_dependencies/robot-description-builder/src/to_rdf/to_sdf.rs
+-rw-r--r--   0     1001      123     2264 2023-06-19 00:27:33.000000 robot_description_builder-0.0.2/local_dependencies/robot-description-builder/src/to_rdf/to_urdf.rs
+-rw-r--r--   0     1001      123     1214 2023-06-19 00:27:33.000000 robot_description_builder-0.0.2/local_dependencies/robot-description-builder/src/to_rdf.rs
+-rw-r--r--   0     1001      123    17462 2023-06-19 00:27:33.000000 robot_description_builder-0.0.2/local_dependencies/robot-description-builder/src/transform.rs
+-rw-r--r--   0     1001      123      652 2023-06-19 00:27:33.000000 robot_description_builder-0.0.2/local_dependencies/robot-description-builder/src/transmission/build_transmission_error.rs
+-rw-r--r--   0     1001      123     5404 2023-06-19 00:27:33.000000 robot_description_builder-0.0.2/local_dependencies/robot-description-builder/src/transmission/hardware_interface.rs
+-rw-r--r--   0     1001      123    16841 2023-06-19 00:27:33.000000 robot_description_builder-0.0.2/local_dependencies/robot-description-builder/src/transmission/mod.rs
+-rw-r--r--   0     1001      123     1955 2023-06-19 00:27:33.000000 robot_description_builder-0.0.2/local_dependencies/robot-description-builder/src/transmission/transmission_actuator.rs
+-rw-r--r--   0     1001      123     4500 2023-06-19 00:27:33.000000 robot_description_builder-0.0.2/local_dependencies/robot-description-builder/src/transmission/transmission_joint.rs
+-rw-r--r--   0     1001      123     1771 2023-06-19 00:27:33.000000 robot_description_builder-0.0.2/local_dependencies/robot-description-builder/src/transmission/transmission_type.rs
+-rw-r--r--   0        0        0      507 1970-01-01 00:00:00.000000 robot_description_builder-0.0.2/Cargo.toml
+-rw-r--r--   0     1001      123      686 2023-06-19 00:27:33.000000 robot_description_builder-0.0.2/.gitignore
+-rw-r--r--   0     1001      123     1073 2023-06-19 00:27:33.000000 robot_description_builder-0.0.2/LICENSE
+-rw-r--r--   0     1001      123     6337 2023-06-19 00:27:33.000000 robot_description_builder-0.0.2/README.md
+-rwxr-xr-x   0     1001      123     5639 2023-06-19 00:27:33.000000 robot_description_builder-0.0.2/examples/urdf-tutorial-05-visual.py
+-rwxr-xr-x   0     1001      123     6090 2023-06-19 00:27:33.000000 robot_description_builder-0.0.2/examples/urdf-tutorial-06-flexible.py
+-rw-r--r--   0     1001      123     1478 2023-06-19 00:27:33.000000 robot_description_builder-0.0.2/pyproject.toml
+-rw-r--r--   0     1001      123      426 2023-06-19 00:27:33.000000 robot_description_builder-0.0.2/python/robot_description_builder/__init__.py
+-rw-r--r--   0     1001      123      865 2023-06-19 00:27:33.000000 robot_description_builder-0.0.2/python/robot_description_builder/__init__.pyi
+-rw-r--r--   0     1001      123      128 2023-06-19 00:27:33.000000 robot_description_builder-0.0.2/python/robot_description_builder/cluster_objects.py
+-rw-r--r--   0     1001      123     1110 2023-06-19 00:27:33.000000 robot_description_builder-0.0.2/python/robot_description_builder/cluster_objects.pyi
+-rw-r--r--   0     1001      123      148 2023-06-19 00:27:33.000000 robot_description_builder-0.0.2/python/robot_description_builder/exceptions.py
+-rw-r--r--   0     1001      123      369 2023-06-19 00:27:33.000000 robot_description_builder-0.0.2/python/robot_description_builder/exceptions.pyi
+-rw-r--r--   0     1001      123      514 2023-06-19 00:27:33.000000 robot_description_builder-0.0.2/python/robot_description_builder/joint.py
+-rw-r--r--   0     1001      123     2953 2023-06-19 00:27:33.000000 robot_description_builder-0.0.2/python/robot_description_builder/joint.pyi
+-rw-r--r--   0     1001      123      245 2023-06-19 00:27:33.000000 robot_description_builder-0.0.2/python/robot_description_builder/link/__init__.py
+-rw-r--r--   0     1001      123     2286 2023-06-19 00:27:33.000000 robot_description_builder-0.0.2/python/robot_description_builder/link/__init__.pyi
+-rw-r--r--   0     1001      123      108 2023-06-19 00:27:33.000000 robot_description_builder-0.0.2/python/robot_description_builder/link/collision.py
+-rw-r--r--   0     1001      123      913 2023-06-19 00:27:33.000000 robot_description_builder-0.0.2/python/robot_description_builder/link/collision.pyi
+-rw-r--r--   0     1001      123      281 2023-06-19 00:27:33.000000 robot_description_builder-0.0.2/python/robot_description_builder/link/geometry.py
+-rw-r--r--   0     1001      123     2332 2023-06-19 00:27:33.000000 robot_description_builder-0.0.2/python/robot_description_builder/link/geometry.pyi
+-rw-r--r--   0     1001      123       95 2023-06-19 00:27:33.000000 robot_description_builder-0.0.2/python/robot_description_builder/link/visual.py
+-rw-r--r--   0     1001      123     1184 2023-06-19 00:27:33.000000 robot_description_builder-0.0.2/python/robot_description_builder/link/visual.pyi
+-rw-r--r--   0     1001      123      717 2023-06-19 00:27:33.000000 robot_description_builder-0.0.2/python/robot_description_builder/material.py
+-rw-r--r--   0     1001      123     1210 2023-06-19 00:27:33.000000 robot_description_builder-0.0.2/python/robot_description_builder/material.pyi
+-rw-r--r--   0     1001      123        0 2023-06-19 00:27:33.000000 robot_description_builder-0.0.2/python/robot_description_builder/py.typed
+-rw-r--r--   0     1001      123      851 2023-06-19 00:27:33.000000 robot_description_builder-0.0.2/python/robot_description_builder/transmission.py
+-rw-r--r--   0     1001      123     1715 2023-06-19 00:27:33.000000 robot_description_builder-0.0.2/python/robot_description_builder/transmission.pyi
+-rw-r--r--   0     1001      123     1325 2023-06-19 00:27:33.000000 robot_description_builder-0.0.2/rdf_builder_py.pyi.old
+-rw-r--r--   0     1001      123       32 2023-06-19 00:27:33.000000 robot_description_builder-0.0.2/requirements-dev.txt
+-rw-r--r--   0     1001      123     3677 2023-06-19 00:27:33.000000 robot_description_builder-0.0.2/src/cluster_objects/kinematic_tree.rs
+-rw-r--r--   0     1001      123     1857 2023-06-19 00:27:33.000000 robot_description_builder-0.0.2/src/cluster_objects/robot.rs
+-rw-r--r--   0     1001      123     4168 2023-06-19 00:27:33.000000 robot_description_builder-0.0.2/src/cluster_objects.rs
+-rw-r--r--   0     1001      123     1070 2023-06-19 00:27:33.000000 robot_description_builder-0.0.2/src/exceptions.rs
+-rw-r--r--   0     1001      123     1634 2023-06-19 00:27:33.000000 robot_description_builder-0.0.2/src/identifier.rs
+-rw-r--r--   0     1001      123     5333 2023-06-19 00:27:33.000000 robot_description_builder-0.0.2/src/joint/base_joint_builder.rs
+-rw-r--r--   0     1001      123     4099 2023-06-19 00:27:33.000000 robot_description_builder-0.0.2/src/joint/generic_joint_builder.rs
+-rw-r--r--   0     1001      123      353 2023-06-19 00:27:33.000000 robot_description_builder-0.0.2/src/joint/smartjointbuilder/fixed_builder.rs
+-rw-r--r--   0     1001      123       41 2023-06-19 00:27:33.000000 robot_description_builder-0.0.2/src/joint/smartjointbuilder/mod.rs
+-rw-r--r--   0     1001      123      382 2023-06-19 00:27:33.000000 robot_description_builder-0.0.2/src/joint/smartjointbuilder/revolute_builder.rs
+-rw-r--r--   0     1001      123     6141 2023-06-19 00:27:33.000000 robot_description_builder-0.0.2/src/joint.rs
+-rw-r--r--   0     1001      123     1277 2023-06-19 00:27:33.000000 robot_description_builder-0.0.2/src/lib.rs
+-rw-r--r--   0     1001      123     4302 2023-06-19 00:27:33.000000 robot_description_builder-0.0.2/src/link/collision.rs
+-rw-r--r--   0     1001      123     2056 2023-06-19 00:27:33.000000 robot_description_builder-0.0.2/src/link/geometry/box_geometry.rs
+-rw-r--r--   0     1001      123     2628 2023-06-19 00:27:33.000000 robot_description_builder-0.0.2/src/link/geometry/cylinder_geometry.rs
+-rw-r--r--   0     1001      123     2912 2023-06-19 00:27:33.000000 robot_description_builder-0.0.2/src/link/geometry/mesh_geometry.rs
+-rw-r--r--   0     1001      123     1855 2023-06-19 00:27:33.000000 robot_description_builder-0.0.2/src/link/geometry/sphere_geometry.rs
+-rw-r--r--   0     1001      123     2991 2023-06-19 00:27:33.000000 robot_description_builder-0.0.2/src/link/geometry.rs
+-rw-r--r--   0     1001      123     2550 2023-06-19 00:27:33.000000 robot_description_builder-0.0.2/src/link/inertial.rs
+-rw-r--r--   0     1001      123     5415 2023-06-19 00:27:33.000000 robot_description_builder-0.0.2/src/link/visual.rs
+-rw-r--r--   0     1001      123    11080 2023-06-19 00:27:33.000000 robot_description_builder-0.0.2/src/link.rs
+-rw-r--r--   0     1001      123     6012 2023-06-19 00:27:33.000000 robot_description_builder-0.0.2/src/material.rs
+-rw-r--r--   0     1001      123     3105 2023-06-19 00:27:33.000000 robot_description_builder-0.0.2/src/to_rdf/to_urdf.rs
+-rw-r--r--   0     1001      123     1186 2023-06-19 00:27:33.000000 robot_description_builder-0.0.2/src/to_rdf.rs
+-rw-r--r--   0     1001      123     4345 2023-06-19 00:27:33.000000 robot_description_builder-0.0.2/src/transform.rs
+-rw-r--r--   0     1001      123     2300 2023-06-19 00:27:33.000000 robot_description_builder-0.0.2/src/transmission/transmission_builder.rs
+-rw-r--r--   0     1001      123     2460 2023-06-19 00:27:33.000000 robot_description_builder-0.0.2/src/transmission/transmission_joint.rs
+-rw-r--r--   0     1001      123     4863 2023-06-19 00:27:33.000000 robot_description_builder-0.0.2/src/transmission/transmission_variants.rs
+-rw-r--r--   0     1001      123     7104 2023-06-19 00:27:33.000000 robot_description_builder-0.0.2/src/transmission/transmission_wrappers.rs
+-rw-r--r--   0     1001      123     4121 2023-06-19 00:27:33.000000 robot_description_builder-0.0.2/src/transmission.rs
+-rw-r--r--   0     1001      123     4721 2023-06-19 00:27:33.000000 robot_description_builder-0.0.2/src/utils.rs
+-rwxr-xr-x   0     1001      123      825 2023-06-19 00:27:33.000000 robot_description_builder-0.0.2/tests/manual-test.py
+-rw-r--r--   0     1001      123     1078 2023-06-19 00:27:33.000000 robot_description_builder-0.0.2/tests/test_geometry.py
+-rw-r--r--   0     1001      123     1086 2023-06-19 00:27:33.000000 robot_description_builder-0.0.2/tests/test_joint.py
+-rw-r--r--   0     1001      123     1079 2023-06-19 00:27:33.000000 robot_description_builder-0.0.2/tests/test_link.py
+-rw-r--r--   0     1001      123      851 2023-06-19 00:27:33.000000 robot_description_builder-0.0.2/tests/test_visual.py
+-rw-r--r--   0     1001      123    17775 2023-06-19 00:27:40.000000 robot_description_builder-0.0.2/Cargo.lock
+-rw-r--r--   0        0        0     7573 1970-01-01 00:00:00.000000 robot_description_builder-0.0.2/PKG-INFO
```

### Comparing `robot_description_builder-0.0.1/local_dependencies/robot-description-builder/LICENSE` & `robot_description_builder-0.0.2/local_dependencies/robot-description-builder/LICENSE`

 * *Files identical despite different names*

### Comparing `robot_description_builder-0.0.1/local_dependencies/robot-description-builder/examples/example-1.rs` & `robot_description_builder-0.0.2/local_dependencies/robot-description-builder/examples/example-1.rs`

 * *Files identical despite different names*

### Comparing `robot_description_builder-0.0.1/local_dependencies/robot-description-builder/examples/smart_builder_example.rs` & `robot_description_builder-0.0.2/local_dependencies/robot-description-builder/examples/smart_builder_example.rs`

 * *Files identical despite different names*

### Comparing `robot_description_builder-0.0.1/local_dependencies/robot-description-builder/examples/transmission-example.rs` & `robot_description_builder-0.0.2/local_dependencies/robot-description-builder/examples/transmission-example.rs`

 * *Files identical despite different names*

### Comparing `robot_description_builder-0.0.1/local_dependencies/robot-description-builder/examples/urdf-tutorial-02.rs` & `robot_description_builder-0.0.2/local_dependencies/robot-description-builder/examples/urdf-tutorial-02.rs`

 * *Files identical despite different names*

### Comparing `robot_description_builder-0.0.1/local_dependencies/robot-description-builder/examples/urdf-tutorial-06-flexible.rs` & `robot_description_builder-0.0.2/local_dependencies/robot-description-builder/examples/urdf-tutorial-05-visual.rs`

 * *Files 24% similar despite different names*

```diff
@@ -1,23 +1,24 @@
+/// If an argument is supplied no meshes are used.
+///
+/// This has been done to prevent allow for the use of an online viewer and the usage of WSL without setting some OpenGL settings.
 use std::{
 	f32::consts::FRAC_PI_2,
 	io::{Read, Seek},
 };
 
-use robot_description_builder as rdb;
-
-use rdb::{
+use robot_description_builder::{
 	link_data::{geometry::*, Visual},
 	material::MaterialDescriptor,
 	prelude::*,
 	to_rdf::{
 		to_urdf::{to_urdf, URDFConfig},
 		XMLMode,
 	},
-	Link, MirrorAxis, Robot, SmartJointBuilder, Transform,
+	JointBuilder, JointType, Link, MirrorAxis, Robot, SmartJointBuilder, Transform,
 };
 
 fn to_urdf_string(robot: &Robot) -> String {
 	let mut buffer = to_urdf(
 		robot,
 		URDFConfig {
 			xml_mode: XMLMode::Indent(' ', 2),
@@ -30,27 +31,31 @@
 	let mut out = String::new();
 	buffer.rewind().unwrap();
 	buffer.read_to_string(&mut out).unwrap();
 
 	out
 }
 
-/// [Building a Movable Robot Model with URDF](http://wiki.ros.org/urdf/Tutorials/Building%20a%20Movable%20Robot%20Model%20with%20URDF)
 fn main() {
+	// Check if we are using meshes, by default meshes are used
+	let args: Vec<String> = std::env::args().collect();
+
+	let use_meshes = args.get(1).is_none();
+
 	/* === Material Descriptions === */
 	let blue_material = MaterialDescriptor::new_rgb(0., 0., 0.8).named("blue");
 	let black_material = MaterialDescriptor::new_rgb(0., 0., 0.).named("black");
 	let white_material = MaterialDescriptor::new_rgb(1., 1., 1.).named("white");
 
 	/* Step 1 */
 	let base_link = Link::builder("base_link").add_visual(
 		Visual::builder(CylinderGeometry::new(0.2, 0.6)).materialized(blue_material.clone()),
 	);
 
-	let model = base_link.build_tree().to_robot("flexible");
+	let model = base_link.build_tree().to_robot("visual");
 
 	/* ====== Start right leg ====== */
 	let right_leg_link = Link::builder("[\\[right]\\]_leg").add_visual(
 		Visual::builder(BoxGeometry::new(0.6, 0.1, 0.2))
 			.materialized(white_material.clone())
 			.tranformed(Transform::new((0., 0., -0.3), (0., FRAC_PI_2, 0.))),
 	);
@@ -73,16 +78,15 @@
 	let right_front_wheel_link = Link::builder("[\\[right]\\]_[[front]]_wheel").add_visual(
 		Visual::builder(CylinderGeometry::new(0.035, 0.1))
 			.tranformed(Transform::new_rotation(FRAC_PI_2, 0., 0.))
 			.materialized(black_material.clone()),
 	);
 
 	let right_front_wheel_joint =
-		SmartJointBuilder::new_continuous("[\\[right]\\]_[[front]]_wheel_joint")
-			.with_axis((0., 1., 0.))
+		SmartJointBuilder::new_fixed("[\\[right]\\]_[[front]]_wheel_joint")
 			.add_transform(Transform::new_translation(0.133333333333, 0., -0.085));
 
 	right_leg
 		.get_newest_link()
 		.write()
 		.unwrap()
 		.try_attach_child(right_front_wheel_link, right_front_wheel_joint)
@@ -92,26 +96,24 @@
 		.get_joint("[\\[right]\\]_[[front]]_wheel_joint")
 		.unwrap()
 		.read()
 		.unwrap()
 		.rebuild_branch()
 		.mirror(MirrorAxis::X);
 	right_back_wheel.change_group_id("back").unwrap();
-	// Need to de-mirror the rotation axis.
-	right_back_wheel.with_axis((0., 1., 0.));
 
 	right_leg
 		.get_link("[\\[right]\\]_base")
 		.unwrap()
 		.write()
 		.unwrap()
 		.attach_joint_chain(right_back_wheel)
 		.unwrap();
 
-	let mut right_leg = right_leg.yank_link("[\\[right]\\]_leg").unwrap();
+	let mut right_leg = right_leg.yank_root();
 	right_leg.apply_group_id();
 
 	let base_right_leg_joint = SmartJointBuilder::new_fixed("base_to_[[right]]_leg")
 		.add_transform(Transform::new_translation(0., -0.22, 0.25));
 
 	/* ==== Attaching right leg ==== */
 
@@ -137,25 +139,101 @@
 		.get_root_link()
 		.write()
 		.unwrap()
 		.attach_joint_chain(left_leg)
 		.unwrap();
 
 	/* === Defining the gripper ==== */
-	// TODO: Meshes
+	let gripper_pole = Link::builder("gripper_pole")
+		.add_visual(
+			Visual::builder(CylinderGeometry::new(0.01, 0.2))
+				.tranformed(Transform::new((0.1, 0., 0.), (0., FRAC_PI_2, 0.))),
+		)
+		.build_tree();
+
+	let left_gripper = Link::builder("[[left]]_gripper")
+		.add_visual(Visual::builder(match use_meshes {
+			true => MeshGeometry::new(
+				"package://urdf_tutorial/meshes/l_finger.dae",
+				(0.1, 0.05, 0.06),
+				None,
+			)
+			.boxed_clone(),
+			false => BoxGeometry::new(0.1, 0.05, 0.06).boxed_clone(),
+		}))
+		.build_tree();
+
+	left_gripper
+		.get_root_link()
+		.write()
+		.unwrap()
+		.try_attach_child(
+			Link::builder("[[left]]_tip").add_visual(
+				Visual::builder(match use_meshes {
+					true => MeshGeometry::new(
+						"package://urdf_tutorial/meshes/l_finger_tip.dae",
+						(0.06, 0.04, 0.02),
+						None,
+					)
+					.boxed_clone(),
+					false => BoxGeometry::new(0.06, 0.04, 0.02).boxed_clone(),
+				})
+				.tranformed(Transform::new_translation(0.09137, 0.00495, 0.)),
+			),
+			SmartJointBuilder::new_fixed("[[left]]_tip_joint"),
+		)
+		.unwrap();
+
+	gripper_pole
+		.get_root_link()
+		.write()
+		.unwrap()
+		.try_attach_child(
+			left_gripper.yank_root(),
+			SmartJointBuilder::new_fixed("[[left]]_gripper_joint")
+				.add_transform(Transform::new_translation(0.2, 0.01, 0.)),
+		)
+		.unwrap();
+
+	let mut right_gripper = gripper_pole
+		.get_joint("[[left]]_gripper_joint")
+		.unwrap()
+		.read()
+		.unwrap()
+		.rebuild_branch()
+		.mirror(MirrorAxis::Y);
+
+	right_gripper.change_group_id("right").unwrap();
+
+	gripper_pole
+		.get_root_link()
+		.write()
+		.unwrap()
+		.attach_joint_chain(right_gripper)
+		.unwrap();
+
+	model
+		.get_root_link()
+		.write()
+		.unwrap()
+		.try_attach_child(
+			gripper_pole.yank_root(),
+			SmartJointBuilder::new_fixed("gripper_extension")
+				.add_transform(Transform::new_translation(0.19, 0., 0.2)),
+		)
+		.unwrap();
 
 	/* ===== Defining the head ===== */
 	let head_link = Link::builder("head").add_visual(
 		Visual::builder(SphereGeometry::new(0.2))
 			.materialized(MaterialDescriptor::new_rgb(1., 1., 1.).named("white")),
 	);
 
-	let head_swivel_joint = SmartJointBuilder::new_continuous("head_swivel")
-		.with_axis((0., 0., 1.))
-		.add_transform(Transform::new_translation(0., 0., 0.3));
+	let head_swivel_joint =
+		JointBuilder::new("head_swivel", JointType::Fixed).add_origin_offset((0., 0., 0.3));
 
 	model
 		.get_root_link()
 		.write()
 		.unwrap()
 		.try_attach_child(head_link, head_swivel_joint)
 		.unwrap();
```

### Comparing `robot_description_builder-0.0.1/local_dependencies/robot-description-builder/src/chained/chained_jointbuilder.rs` & `robot_description_builder-0.0.2/local_dependencies/robot-description-builder/src/chained/chained_jointbuilder.rs`

 * *Files 6% similar despite different names*

```diff
@@ -350,8 +350,27 @@
 				}),
 				..Default::default()
 			})
 		);
 
 		assert_eq!(left_leg_builder, right_leg_builder_z.mirror(MirrorAxis::Z));
 	}
+
+	// #[test]
+	// fn chained_escaping() {
+	// 	let tree = Link::builder("root-link").build_tree();
+
+	// 	tree.get_root_link()
+	// 		.try_write()
+	// 		.unwrap()
+	// 		.try_attach_child(
+	// 			Link::builder("child-link")
+	// 				.add_visual(Visual::builder(BoxGeometry::new(3., 4., 5.))),
+	// 			SmartJointBuilder::new_continuous("jointy"),
+	// 		)
+	// 		.unwrap();
+
+	// 	let mut builder = tree.yank_root();
+
+	// 	builder.add_visual(Visual::builder(BoxGeometry::new(2.,3.,4.)));
+	// }
 }
```

### Comparing `robot_description_builder-0.0.1/local_dependencies/robot-description-builder/src/chained/chained_linkbuilder.rs` & `robot_description_builder-0.0.2/local_dependencies/robot-description-builder/src/chained/chained_linkbuilder.rs`

 * *Files 0% similar despite different names*

```diff
@@ -66,16 +66,15 @@
 
 impl<KI> From<KI> for Chained<LinkBuilder>
 where
 	KI: KinematicInterface,
 {
 	fn from(value: KI) -> Self {
 		// FIXME: Is unwrap Ok Here?
-		// FIXME: Maybe use the non-blocking read, for production?
-		Self(value.get_root_link().try_read().unwrap().yank())
+		Self(value.get_root_link().read().unwrap().yank())
 	}
 }
 
 #[cfg(test)]
 mod tests {
 	use std::f32::consts::FRAC_PI_2;
```

### Comparing `robot_description_builder-0.0.1/local_dependencies/robot-description-builder/src/chained/mod.rs` & `robot_description_builder-0.0.2/local_dependencies/robot-description-builder/src/chained/mod.rs`

 * *Files 10% similar despite different names*

```diff
@@ -7,52 +7,56 @@
 };
 
 use crate::identifiers::GroupIDChanger;
 
 #[derive(Debug, PartialEq, Clone)]
 pub struct Chained<Builder: ChainableBuilder>(pub(crate) Builder);
 
-impl<Builder> Chained<Builder>
-where
-	Builder: ChainableBuilder,
-{
-	/// TODO: Maybe deprecate
-	pub fn builder(&self) -> &Builder {
-		&self.0
-	}
-
-	/// FIXME: This is not very usefull since most JointBuilder Methods are consuming
-	/// TODO: Maybe deprecate
-	pub fn builder_mut(&mut self) -> &mut Builder {
-		&mut self.0
-	}
-
-	/// TODO: Maybe deprecate since Deref and DerefMut
-	/// Allows the internal `Builder` and it's chain to be changed by a closure.
-	///
-	/// If in this process the `Builder` has lost it's chain, for example due to overwriting.
-	/// An error of type `Builder` is retured so the updated `Builder` can still be used.
-	pub fn modify_builder<F>(self, mut f: F) -> Result<Self, Builder>
-	where
-		F: FnMut(Builder) -> Builder,
-	{
-		let builder = f(self.0);
-
-		// When we are tricked into loosing our chain
-		match builder.has_chain() {
-			// The modified `Builder` still has a chain, therefor we can continue to assume our `Builder` has a chain and make a new `Chained<Builder>`.
-			true => Ok(Self(builder)),
-			// The modified `Builder` has does not have a chain, therefor we can not build chains with it.
-			false => Err(builder),
-		}
-	}
-}
+// impl<Builder> Chained<Builder>
+// where
+// 	Builder: ChainableBuilder,
+// {
+// 	/// TODONE: Maybe deprecate
+// 	pub fn builder(&self) -> &Builder {
+// 		&self.0
+// 	}
+
+// 	/// FIXEDME: This is not very usefull since most JointBuilder Methods are consuming
+// 	/// TODONE: Maybe deprecate
+// 	pub fn builder_mut(&mut self) -> &mut Builder {
+// 		&mut self.0
+// 	}
+
+// 	/// TODONE: Maybe deprecate since Deref and DerefMut
+// 	/// Allows the internal `Builder` and it's chain to be changed by a closure.
+// 	///
+// 	/// If in this process the `Builder` has lost it's chain, for example due to overwriting.
+// 	/// An error of type `Builder` is retured so the updated `Builder` can still be used.
+// 	pub fn modify_builder<F>(self, mut f: F) -> Result<Self, Builder>
+// 	where
+// 		F: FnMut(Builder) -> Builder,
+// 	{
+// 		let builder = f(self.0);
+
+// 		// When we are tricked into loosing our chain
+// 		match builder.has_chain() {
+// 			// The modified `Builder` still has a chain, therefor we can continue to assume our `Builder` has a chain and make a new `Chained<Builder>`.
+// 			true => Ok(Self(builder)),
+// 			// The modified `Builder` has does not have a chain, therefor we can not build chains with it.
+// 			false => Err(builder),
+// 		}
+// 	}
+// }
 
 // To allow for calling functions on the internal builders
 // TODO: Figure out if builderfunctions do not free the internal builder from it `Chained<Builder>` Identifier
+//
+// UPDATE: We do not escape however, the functions that consume can not be called either, see test chained::chained_joint_builder::test::chained escaping
+// TODO: Solution?: Add inplace methods???
+//
 // FIXME: but deref should theoretically only be implemented for smartpointers which do not add methods
 // https://rust-lang.github.io/api-guidelines/predictability.html?highlight=deref#only-smart-pointers-implement-deref-and-derefmut-c-deref
 // https://rust-lang.github.io/api-guidelines/predictability.html?highlight=deref#smart-pointers-do-not-add-inherent-methods-c-smart-ptr
 impl<Builder> Deref for Chained<Builder>
 where
 	Builder: ChainableBuilder,
 {
@@ -70,14 +74,25 @@
 	Builder: ChainableBuilder,
 {
 	fn deref_mut(&mut self) -> &mut Self::Target {
 		&mut self.0
 	}
 }
 
+#[cfg(feature = "wrapper")]
+impl<Builder> Chained<Builder>
+where
+	Builder: ChainableBuilder,
+{
+	/// Create a Chained Builder, needs to be a chain.
+	pub unsafe fn new(builder: Builder) -> Self {
+		Chained(builder)
+	}
+}
+
 pub trait ChainableBuilder: Debug + PartialEq + Clone + GroupIDChanger {
 	/// Returns `true` if the builder has a chain/one or more childeren.
 	fn has_chain(&self) -> bool;
 }
 
 #[cfg(test)]
 mod tests {
```

### Comparing `robot_description_builder-0.0.1/local_dependencies/robot-description-builder/src/cluster_objects/kinematic_data_errors.rs` & `robot_description_builder-0.0.2/local_dependencies/robot-description-builder/src/cluster_objects/kinematic_data_errors.rs`

 * *Files identical despite different names*

### Comparing `robot_description_builder-0.0.1/local_dependencies/robot-description-builder/src/cluster_objects/kinematic_data_tree.rs` & `robot_description_builder-0.0.2/local_dependencies/robot-description-builder/src/cluster_objects/kinematic_data_tree.rs`

 * *Files 0% similar despite different names*

```diff
@@ -51,15 +51,15 @@
 		});
 
 		{
 			#[cfg(any(feature = "logging", test))]
 			log::trace!("Attempting to register tree data to index");
 
 			// 1st Unwrapping is Ok here, since we just made the KinematicDataTree
-			data.try_add_link(&data.root_link).unwrap(); //FIXME: 2nd Unwrap Ok?
+			data.try_add_link(&data.root_link).unwrap(); //FIXME: is Unwrap Ok? No Link could contain conflicting materials
 		}
 		data
 	}
 
 	pub(crate) fn try_add_material(&self, material: &mut Material) -> Result<(), AddMaterialError> {
 		material.initialize(self)
 	}
```

### Comparing `robot_description_builder-0.0.1/local_dependencies/robot-description-builder/src/cluster_objects/kinematic_tree.rs` & `robot_description_builder-0.0.2/local_dependencies/robot-description-builder/src/cluster_objects/kinematic_tree.rs`

 * *Files 1% similar despite different names*

```diff
@@ -77,15 +77,15 @@
 	fn get_material(&self, name: &str) -> Option<Material> {
 		self.0
 			.material_index
 			.read()
 			.unwrap() // FIXME: Unwrapping might not be ok
 			.get(name)
 			.map(Arc::clone)
-			.map(|data| (name.into(), data).into())
+			.map(|data| Material::new_named_inited(name, data))
 	}
 
 	fn get_transmission(&self, name: &str) -> Option<ArcLock<Transmission>> {
 		self.0
 			.transmissions
 			.read()
 			.unwrap() // FIXME: Unwrapping might not be ok
@@ -126,27 +126,21 @@
 }
 
 impl Clone for KinematicTree {
 	fn clone(&self) -> Self {
 		let root_link = self
 			.get_root_link()
 			.read()
-			.unwrap()
-			.rebuild_branch_continued(); // FIXME: UNWRAP MIGHTN NOT BE OK HERE
+			.unwrap() // FIXME: UNWRAP MIGHTN NOT BE OK HERE
+			.rebuild_branch_continued();
 
 		root_link.build_tree()
 	}
 }
 
-impl From<KinematicTree> for Box<dyn KinematicInterface> {
-	fn from(value: KinematicTree) -> Self {
-		Box::new(value)
-	}
-}
-
 #[cfg(test)]
 mod tests {
 	use log::trace;
 	use std::sync::{Arc, Weak};
 	use test_log::test;
 
 	use crate::{
@@ -187,24 +181,24 @@
 			&cloned_tree.get_root_link()
 		));
 
 		// Note: This may not be permanent behavior
 		trace!(
 			target: "RDB-RS::test::KineTree::clone_single",
 			"tree->..->root_link->name        | ptr: {:#?}",
-			&tree.get_root_link().try_read().unwrap().name.as_ptr()
+			&tree.get_root_link().try_read().unwrap().name().as_ptr()
 		);
 		trace!(
 			target: "RDB-RS::test::KineTree::clone_single",
 			"cloned_tree->..->root_link->name | ptr: {:#?}\n",
 			&cloned_tree
 				.get_root_link()
 				.try_read()
 				.unwrap()
-				.name
+				.name()
 				.as_ptr()
 		);
 		assert_eq!(
 			&tree.get_root_link().try_read().unwrap().name(),
 			&cloned_tree.get_root_link().try_read().unwrap().name()
 		);
 
@@ -445,24 +439,24 @@
 			&cloned_tree.get_root_link()
 		));
 
 		// Note: This may not be permanent behavior
 		trace!(
 			target: "RDB-RS::test::KineTree::clone_multi",
 			"tree->..->root_link->name        | ptr: {:#?}",
-			&tree.get_root_link().try_read().unwrap().name.as_ptr()
+			&tree.get_root_link().try_read().unwrap().name().as_ptr()
 		);
 		trace!(
 			target: "RDB-RS::test::KineTree::clone_multi",
 			"cloned_tree->..->root_link->name | ptr: {:#?}\n",
 			&cloned_tree
 				.get_root_link()
 				.try_read()
 				.unwrap()
-				.name
+				.name()
 				.as_ptr()
 		);
 		assert_eq!(
 			&tree.get_root_link().try_read().unwrap().name(),
 			&cloned_tree.get_root_link().try_read().unwrap().name()
 		);
```

### Comparing `robot_description_builder-0.0.1/local_dependencies/robot-description-builder/src/cluster_objects/robot.rs` & `robot_description_builder-0.0.2/local_dependencies/robot-description-builder/src/cluster_objects/robot.rs`

 * *Files 5% similar despite different names*

```diff
@@ -101,15 +101,15 @@
 	fn get_material(&self, name: &str) -> Option<Material> {
 		self.data
 			.material_index
 			.read()
 			.unwrap() // FIXME: Unwrapping might not be ok
 			.get(name)
 			.map(Arc::clone)
-			.map(|data| (name.to_string(), data).into())
+			.map(|data| Material::new_named_inited(name, data))
 	}
 
 	fn get_transmission(&self, name: &str) -> Option<ArcLock<Transmission>> {
 		self.data
 			.transmissions
 			.read()
 			.unwrap() // FIXME: Unwrapping might not be ok
@@ -160,13 +160,7 @@
 			key: QName(b"name"),
 			value: self.name.display().as_bytes().into(),
 		});
 		element.write_inner_content(|writer| self.data.to_urdf(writer, urdf_config))?;
 		Ok(())
 	}
 }
-
-impl From<Robot> for Box<dyn KinematicInterface> {
-	fn from(value: Robot) -> Self {
-		Box::new(value)
-	}
-}
```

### Comparing `robot_description_builder-0.0.1/local_dependencies/robot-description-builder/src/cluster_objects.rs` & `robot_description_builder-0.0.2/local_dependencies/robot-description-builder/src/cluster_objects.rs`

 * *Files 9% similar despite different names*

```diff
@@ -21,16 +21,15 @@
 mod robot;
 
 pub use kinematic_tree::KinematicTree;
 pub use robot::Robot;
 
 type PoisonWriteIndexError<'a, K, V> = PoisonError<RwLockWriteGuard<'a, HashMap<K, V>>>;
 
-/// TODO: MAYBE RENAME SOME FUNCTIONS to conform to convention
-pub trait KinematicInterface {
+pub trait KinematicInterface: Sized {
 	// NOTE: THIS IS NOT FINAL;
 
 	/// Returns the root link of the Kinematic Tree
 	///
 	/// # Example
 	/// ```
 	/// # use robot_description_builder::{KinematicInterface, Link, JointBuilder, JointType, linkbuilding::LinkBuilder};
@@ -91,16 +90,14 @@
 	/// TODO: NOT FINAL
 	/// TODO: Maybe remove rcrefcell from transmission parameter
 	fn try_add_transmission(
 		&self,
 		transmission: TransmissionBuilder<WithJoints, WithActuator>,
 	) -> Result<(), AddTransmissionError>;
 
-	// TODO: Expand
-
 	/// Cleans up orphaned/broken `Link` entries from the `links` HashMap.
 	///
 	/// This mostly happens automatically, but is exposed for use in other methods.
 	///
 	/// TODO: DOCTEST/EXAMPLE
 	fn purge_links(&self) -> Result<(), PoisonWriteIndexError<String, WeakLock<Link>>>;
 
@@ -128,19 +125,40 @@
 			.map(|link| link.read().unwrap().yank()) // FIXME: Is unwrap ok here?
 			.map(Chained);
 		self.purge_joints().unwrap(); // FIXME: Is unwrap ok here?
 		self.purge_links().unwrap(); // FIXME: Is unwrap ok here?
 		builder
 	}
 
+	/// Cosumes the `KinematicInterface` implementor and creates a `Chained<LinkBuilder>` to rebuild it.
+	///
+	/// This has the same result as yanking the `root_link`, with the additional effect that the current tree is consumed.
+	///
+	/// # Example
+	///
+	/// ```
+	/// # use robot_description_builder::{prelude::*, Link};
+	///
+	/// let builder = Link::builder("root-link");
+	///
+	/// assert_eq!(*builder.clone().build_tree().yank_root(), builder);
+	///
+	/// /// It is equivalent to yanking the "root_link"
+	/// assert_eq!(builder.clone().build_tree().yank_root(), builder.build_tree().yank_link("root-link").unwrap())
+	/// ```
+	fn yank_root(self) -> Chained<LinkBuilder> {
+		let builder = self.get_root_link().read().unwrap().yank();
+		Chained(builder)
+	}
+
 	fn yank_joint(&self, name: &str) -> Option<Chained<JointBuilder>> {
 		let builder = self
 			.get_joint(name)
 			.map(|joint| joint.read().unwrap().yank()) // FIXME: Is unwrap ok here?
 			.map(Chained);
 		self.purge_joints().unwrap(); // FIXME: Is unwrap ok here?
 		self.purge_links().unwrap(); // FIXME: Is unwrap ok here?
 		builder
 	}
 
-	// TODO: MAYBE yank_root or a rebuild?
+	// TODO: or a rebuild?
 }
```

### Comparing `robot_description_builder-0.0.1/local_dependencies/robot-description-builder/src/identifiers.rs` & `robot_description_builder-0.0.2/local_dependencies/robot-description-builder/src/identifiers.rs`

 * *Files identical despite different names*

### Comparing `robot_description_builder-0.0.1/local_dependencies/robot-description-builder/src/joint/joint_data/calibration_data.rs` & `robot_description_builder-0.0.2/local_dependencies/robot-description-builder/src/joint/joint_data/calibration_data.rs`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #[cfg(feature = "xml")]
 use quick_xml::{events::attributes::Attribute, name::QName};
 
 #[derive(Debug, PartialEq, Clone, Copy, Default)]
-/// TODO: maybe change visibilty
+/// TODO: DOC
 pub struct CalibrationData {
 	pub rising: Option<f32>,
 	pub falling: Option<f32>,
 }
 
 impl CalibrationData {
 	/// A function to check if any of the fields are set.
```

### Comparing `robot_description_builder-0.0.1/local_dependencies/robot-description-builder/src/joint/joint_data/dynamics_data.rs` & `robot_description_builder-0.0.2/local_dependencies/robot-description-builder/src/joint/joint_data/dynamics_data.rs`

 * *Files identical despite different names*

### Comparing `robot_description_builder-0.0.1/local_dependencies/robot-description-builder/src/joint/joint_data/limit_data.rs` & `robot_description_builder-0.0.2/local_dependencies/robot-description-builder/src/joint/joint_data/limit_data.rs`

 * *Files identical despite different names*

### Comparing `robot_description_builder-0.0.1/local_dependencies/robot-description-builder/src/joint/joint_data/mimic_data.rs` & `robot_description_builder-0.0.2/local_dependencies/robot-description-builder/src/joint/joint_data/mimic_data.rs`

 * *Files identical despite different names*

### Comparing `robot_description_builder-0.0.1/local_dependencies/robot-description-builder/src/joint/joint_data/safety_controller_data.rs` & `robot_description_builder-0.0.2/local_dependencies/robot-description-builder/src/joint/joint_data/safety_controller_data.rs`

 * *Files identical despite different names*

### Comparing `robot_description_builder-0.0.1/local_dependencies/robot-description-builder/src/joint/joint_tranform_mode.rs` & `robot_description_builder-0.0.2/local_dependencies/robot-description-builder/src/joint/joint_tranform_mode.rs`

 * *Files identical despite different names*

### Comparing `robot_description_builder-0.0.1/local_dependencies/robot-description-builder/src/joint/jointbuilder.rs` & `robot_description_builder-0.0.2/local_dependencies/robot-description-builder/src/joint/jointbuilder.rs`

 * *Files 15% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 	cluster_objects::kinematic_data_tree::KinematicDataTree,
 	identifiers::GroupIDChanger,
 	joint::{joint_data, joint_tranform_mode::JointTransformMode, Joint, JointType},
 	link::{
 		builder::{BuildLink, LinkBuilder},
 		Link, LinkShapeData,
 	},
-	transform::{Mirror, MirrorUpdater},
+	transform::{Mirror, MirrorUpdater, Transform},
 	ArcLock, WeakLock,
 };
 
 pub trait BuildJoint: Into<JointBuilder> {
 	/// Creates the joint ?? and subscribes it to the right right places
 	fn build(
 		self,
@@ -35,54 +35,62 @@
 		parent_shape_data: LinkShapeData,
 	) -> ArcLock<Joint>;
 }
 
 #[derive(Debug, PartialEq, Clone, Default)]
 pub struct JointBuilder {
 	pub(crate) name: String,
-	pub(crate) joint_type: JointType, // TODO: FINISH ME
+	pub(crate) joint_type: JointType,
 	/// TODO: Maybe add a Figure it out???
 	pub(crate) origin: JointTransformMode,
 	pub(crate) child: Option<LinkBuilder>,
 
-	/// TODO: DO SOMETHING WITH THIS
+	//Consider making everything below pub to remove need for all the functions
 	/// TODO: MAYBE CHANGE TO Vec3D Or something
 	pub(crate) axis: Option<(f32, f32, f32)>,
 	pub(crate) calibration: joint_data::CalibrationData,
 	pub(crate) dynamics: joint_data::DynamicsData,
 	pub(crate) limit: Option<joint_data::LimitData>,
 	pub(crate) mimic: Option<joint_data::MimicBuilderData>,
 	pub(crate) safety_controller: Option<joint_data::SafetyControllerData>,
 }
 
+/// TODO: maybe add new_full ? or make fields public
 impl JointBuilder {
 	pub fn new(name: impl Into<String>, joint_type: JointType) -> Self {
 		Self {
 			name: name.into(),
 			joint_type,
 			..Default::default()
 		}
 	}
 
+	/// TODO: rename transform
 	pub fn add_origin_offset(mut self, offset: (f32, f32, f32)) -> Self {
 		match &mut self.origin {
 			JointTransformMode::Direct(transform) => transform.translation = Some(offset),
 			JointTransformMode::FigureItOut(_) => todo!("Don't know how to do this"),
 		};
 		self
 	}
 
+	/// TODO: rename transform
 	pub fn add_origin_rotation(mut self, rotation: (f32, f32, f32)) -> Self {
 		match &mut self.origin {
 			JointTransformMode::Direct(tranform) => tranform.rotation = Some(rotation),
 			JointTransformMode::FigureItOut(_) => todo!("Don't know how to do this yet"),
 		}
 		self
 	}
 
+	pub fn set_transform_simple(&mut self, transform: Transform) {
+		self.origin = JointTransformMode::Direct(transform);
+	}
+
+	/// TODO: rename transform
 	/// Nominated for Deprication
 	/// Maybe Not??
 	#[inline]
 	pub(crate) fn with_origin<JTM>(&mut self, origin: JTM)
 	where
 		JTM: Into<JointTransformMode>,
 	{
@@ -121,14 +129,102 @@
 		&mut self,
 		safety_controller_data: joint_data::SafetyControllerData,
 	) {
 		self.safety_controller = Some(safety_controller_data);
 	}
 }
 
+// Mostly for Python Wrapper
+/// Non Builder functions
+impl JointBuilder {
+	pub fn name(&self) -> &String {
+		&self.name
+	}
+
+	pub fn joint_type(&self) -> &JointType {
+		&self.joint_type
+	}
+
+	pub fn transform(&self) -> Option<&Transform> {
+		// TODO: Maybe add a advanced mode for figure it out?
+		match &self.origin {
+			JointTransformMode::Direct(transform) => match transform.contains_some() {
+				true => Some(transform),
+				false => None,
+			},
+			JointTransformMode::FigureItOut(_) => todo!("?"),
+		}
+	}
+
+	pub fn transform_mut(&mut self) -> Option<&mut Transform> {
+		// TODO: Maybe add a advanced mode for figure it out?
+		match &mut self.origin {
+			JointTransformMode::Direct(transform) => match transform.contains_some() {
+				true => Some(transform),
+				false => None,
+			},
+			JointTransformMode::FigureItOut(_) => todo!("?"),
+		}
+	}
+
+	// TODO: ORIGIN
+
+	pub fn child(&self) -> Option<&LinkBuilder> {
+		self.child.as_ref()
+	}
+
+	pub fn axis(&self) -> Option<(f32, f32, f32)> {
+		self.axis
+	}
+
+	pub fn axis_mut(&mut self) -> Option<&mut (f32, f32, f32)> {
+		self.axis.as_mut()
+	}
+
+	pub fn calibration(&self) -> &joint_data::CalibrationData {
+		&self.calibration
+	}
+
+	pub fn calibration_mut(&mut self) -> &mut joint_data::CalibrationData {
+		&mut self.calibration
+	}
+
+	pub fn dynamics(&self) -> &joint_data::DynamicsData {
+		&self.dynamics
+	}
+
+	pub fn dynamics_mut(&mut self) -> &mut joint_data::DynamicsData {
+		&mut self.dynamics
+	}
+
+	pub fn limit(&self) -> Option<&joint_data::LimitData> {
+		self.limit.as_ref()
+	}
+
+	pub fn limit_mut(&mut self) -> &mut Option<joint_data::LimitData> {
+		&mut self.limit
+	}
+
+	pub fn mimic(&self) -> Option<&joint_data::MimicBuilderData> {
+		self.mimic.as_ref()
+	}
+
+	pub fn mimic_mut(&mut self) -> &mut Option<joint_data::MimicBuilderData> {
+		&mut self.mimic
+	}
+
+	pub fn safety_controller(&self) -> Option<&joint_data::SafetyControllerData> {
+		self.safety_controller.as_ref()
+	}
+
+	pub fn safety_controller_mut(&mut self) -> &mut Option<joint_data::SafetyControllerData> {
+		&mut self.safety_controller
+	}
+}
+
 impl Mirror for JointBuilder {
 	fn mirrored(&self, mirror_matrix: &Matrix3<f32>) -> Self {
 		let (origin, new_mirror_matrix) = self.origin.mirrored_update_matrix(mirror_matrix);
 		Self {
 			name: self.name.clone(), // FIXME: Rename
 			joint_type: self.joint_type,
 			origin,
@@ -136,19 +232,21 @@
 				.child
 				.as_ref()
 				.map(|link_builder| link_builder.mirrored(&new_mirror_matrix)),
 			axis: match (self.joint_type, self.axis) {
 				(JointType::Fixed | JointType::Floating, _) => None, // TODO: Figure out if this clause should be moved down to allow for Fixed and Floating with axis if desired?
 				(_, Some((x, y, z))) => Some(
 					(new_mirror_matrix * vector![x, y, z] * -1.)
-						.normalize() // Theoretically not necessary, but float rounding errors are a thing | TODO: Figure out if this improves the situation or makes it worse
+						// Theoretically not necessary, but float rounding errors are a thing | TODO: Figure out if this improves the situation or makes it worse
+						.normalize()
 						.iter()
 						.copied()
 						.collect_tuple()
-						.unwrap(), // Unwrapping here to ensure that we collect to a Tuple3 | TODO: Change to expect? or remove
+						// Unwrapping here to ensure that we collect to a Tuple3 | TODO: Change to expect? or remove
+						.unwrap(),
 				),
 				(
 					JointType::Revolute
 					| JointType::Continuous
 					| JointType::Prismatic
 					| JointType::Planar,
 					None,
@@ -157,19 +255,19 @@
 						.normalize() // Theoretically not necessary, but float rounding errors are a thing | TODO: Figure out if this improves the situation or makes it worse
 						.iter()
 						.copied()
 						.collect_tuple()
 						.unwrap(), // Unwrapping here to ensure that we collect to a Tuple3 | TODO: Change to expect? or remove
 				),
 			},
-			calibration: self.calibration,                // TODO: Is this Correct?
-			dynamics: self.dynamics,                      // TODO: Is this Correct?
-			limit: self.limit,                            // TODO: Is this Correct?
-			mimic: self.mimic.as_ref().map(Clone::clone), // TODO: Is this Correct?
-			safety_controller: self.safety_controller,    // TODO: Is this Correct?
+			calibration: self.calibration,             // TODO: Is this Correct?
+			dynamics: self.dynamics,                   // TODO: Is this Correct?
+			limit: self.limit,                         // TODO: Is this Correct?
+			mimic: self.mimic.as_ref().cloned(),       // TODO: Is this Correct?
+			safety_controller: self.safety_controller, // TODO: Is this Correct?
 		}
 	}
 }
 
 impl BuildJoint for JointBuilder {
 	fn build(
 		self,
```

### Comparing `robot_description_builder-0.0.1/local_dependencies/robot-description-builder/src/joint/smartjointbuilder/smartjointtypes/continuous_joint_type.rs` & `robot_description_builder-0.0.2/local_dependencies/robot-description-builder/src/joint/smartjointbuilder/smartjointtypes/continuous_joint_type.rs`

 * *Files 4% similar despite different names*

```diff
@@ -1,23 +1,28 @@
 use std::sync::Weak;
 
 use crate::{
 	cluster_objects::kinematic_data_tree::KinematicDataTree,
 	joint::{
 		jointbuilder::{BuildJoint, JointBuilder},
-		smartjointbuilder::smartparams::{smart_joint_datatraits, smart_joint_specification},
+		smartjointbuilder::smartparams::{
+			smart_joint_datatraits::{self, JointTypeTrait},
+			smart_joint_specification,
+		},
 		Joint, JointType, SmartJointBuilder,
 	},
 	link::Link,
 	ArcLock, WeakLock,
 };
 
 #[derive(Debug, PartialEq, Eq, Clone, Copy, Default)]
 pub struct ContinuousType;
 
+impl_jointtype_traits!(ContinuousType, true);
+
 impl From<ContinuousType> for JointType {
 	fn from(_value: ContinuousType) -> Self {
 		JointType::Continuous
 	}
 }
 
 impl smart_joint_specification::AxisAllowed for ContinuousType {}
@@ -83,14 +88,16 @@
 		let mut joint_builder = JointBuilder::new(value.name, value.joint_type.into());
 
 		joint_builder.with_origin(value.origin.unwrap_or_default());
 
 		value.axis.simplify(&mut joint_builder);
 		value.calibration.simplify(&mut joint_builder);
 		value.dynamics.simplify(&mut joint_builder);
-		value.limit.simplify(&mut joint_builder, true);
+		value
+			.limit
+			.simplify(&mut joint_builder, ContinuousType::IS_CONTINOUS);
 		value.mimic.simplify(&mut joint_builder);
 		value.safety_controller.simplify(&mut joint_builder);
 
 		joint_builder
 	}
 }
```

### Comparing `robot_description_builder-0.0.1/local_dependencies/robot-description-builder/src/joint/smartjointbuilder/smartjointtypes/fixed_joint_type.rs` & `robot_description_builder-0.0.2/local_dependencies/robot-description-builder/src/joint/smartjointbuilder/smartjointtypes/fixed_joint_type.rs`

 * *Files 10% similar despite different names*

```diff
@@ -15,14 +15,16 @@
 	link::Link,
 	ArcLock, WeakLock,
 };
 
 #[derive(Debug, PartialEq, Eq, Clone, Copy, Default)]
 pub struct FixedType;
 
+impl_jointtype_traits!(FixedType, false);
+
 impl From<FixedType> for JointType {
 	fn from(_value: FixedType) -> Self {
 		JointType::Fixed
 	}
 }
 
 impl BuildJoint
```

### Comparing `robot_description_builder-0.0.1/local_dependencies/robot-description-builder/src/joint/smartjointbuilder/smartjointtypes/floating_joint_type.rs` & `robot_description_builder-0.0.2/local_dependencies/robot-description-builder/src/joint/smartjointbuilder/smartjointtypes/floating_joint_type.rs`

 * *Files 3% similar despite different names*

```diff
@@ -35,14 +35,16 @@
 ///
 /// ## Extra sources:
 /// - [GitHub:URDF/issue/Support for other joint types](https://github.com/ros/urdf/issues/3)
 /// - [Gazebo uses KDL, so doesn't support Floating](https://get-help.robotigniteacademy.com/t/urdfs-floating-joint-not-working-in-gazebo/8864)
 #[derive(Debug, PartialEq, Eq, Clone, Copy, Default)]
 pub struct FloatingType;
 
+impl_jointtype_traits!(FloatingType, false);
+
 impl From<FloatingType> for JointType {
 	fn from(_value: FloatingType) -> Self {
 		JointType::Floating
 	}
 }
 
 // Axis is not allowed
@@ -105,14 +107,16 @@
 
 		joint_builder.with_origin(value.origin.unwrap_or_default());
 
 		// Probably unneccessary
 		value.axis.simplify(&mut joint_builder);
 		value.calibration.simplify(&mut joint_builder);
 		value.dynamics.simplify(&mut joint_builder);
-		value.limit.simplify(&mut joint_builder, false);
+		value
+			.limit
+			.simplify(&mut joint_builder, FloatingType::IS_CONTINOUS);
 		value.mimic.simplify(&mut joint_builder);
 		value.safety_controller.simplify(&mut joint_builder);
 
 		joint_builder
 	}
 }
```

### Comparing `robot_description_builder-0.0.1/local_dependencies/robot-description-builder/src/joint/smartjointbuilder/smartjointtypes/planar_joint_type.rs` & `robot_description_builder-0.0.2/local_dependencies/robot-description-builder/src/joint/smartjointbuilder/smartjointtypes/planar_joint_type.rs`

 * *Files 6% similar despite different names*

```diff
@@ -1,26 +1,31 @@
 use std::sync::Weak;
 
 use crate::{
 	cluster_objects::kinematic_data_tree::KinematicDataTree,
 	joint::{
 		jointbuilder::{BuildJoint, JointBuilder},
 		smartjointbuilder::{
-			smartparams::{smart_joint_datatraits, smart_joint_specification},
+			smartparams::{
+				smart_joint_datatraits::{self, JointTypeTrait},
+				smart_joint_specification,
+			},
 			SmartJointBuilder,
 		},
 		Joint, JointType,
 	},
 	link::Link,
 	ArcLock, WeakLock,
 };
 
 #[derive(Debug, PartialEq, Eq, Clone, Copy, Default)]
 pub struct PlanarType;
 
+impl_jointtype_traits!(PlanarType, true); // FIXME: Is it continous?
+
 impl From<PlanarType> for JointType {
 	fn from(_value: PlanarType) -> Self {
 		JointType::Planar
 	}
 }
 
 impl smart_joint_specification::AxisAllowed for PlanarType {}
@@ -80,14 +85,16 @@
 		let mut joint_builder = JointBuilder::new(value.name, value.joint_type.into());
 
 		joint_builder.with_origin(value.origin.unwrap_or_default());
 
 		value.axis.simplify(&mut joint_builder);
 		value.calibration.simplify(&mut joint_builder);
 		value.dynamics.simplify(&mut joint_builder);
-		value.limit.simplify(&mut joint_builder, true); // FIXME: Is it contiuos tho?
+		value
+			.limit
+			.simplify(&mut joint_builder, PlanarType::IS_CONTINOUS);
 		value.mimic.simplify(&mut joint_builder);
 		value.safety_controller.simplify(&mut joint_builder);
 
 		joint_builder
 	}
 }
```

### Comparing `robot_description_builder-0.0.1/local_dependencies/robot-description-builder/src/joint/smartjointbuilder/smartjointtypes/prismatic_joint_type.rs` & `robot_description_builder-0.0.2/local_dependencies/robot-description-builder/src/joint/smartjointbuilder/smartjointtypes/prismatic_joint_type.rs`

 * *Files 4% similar despite different names*

```diff
@@ -2,31 +2,33 @@
 
 use crate::{
 	cluster_objects::kinematic_data_tree::KinematicDataTree,
 	joint::{
 		jointbuilder::{BuildJoint, JointBuilder},
 		smartjointbuilder::{
 			smartparams::{
-				smart_joint_datatraits::{self, LimitDataType},
+				smart_joint_datatraits::{self, JointTypeTrait, LimitDataType},
 				smart_joint_specification, WithLimit,
 			},
 			SmartJointBuilder,
 		},
 		Joint, JointType,
 	},
 	link::Link,
 	ArcLock, WeakLock,
 };
 
 #[derive(Debug, PartialEq, Eq, Clone, Copy, Default)]
 pub struct PrismaticType;
 
+impl_jointtype_traits!(PrismaticType, false);
+
 impl From<PrismaticType> for JointType {
 	fn from(_value: PrismaticType) -> Self {
-		JointType::Continuous
+		JointType::Prismatic
 	}
 }
 
 impl smart_joint_specification::AxisAllowed for PrismaticType {}
 impl smart_joint_specification::CalibrationAllowed for PrismaticType {}
 impl smart_joint_specification::DynamicsAllowed for PrismaticType {}
 impl smart_joint_specification::LimitAllowed for PrismaticType {}
@@ -93,14 +95,16 @@
 		let mut joint_builder = JointBuilder::new(value.name, value.joint_type.into());
 
 		joint_builder.with_origin(value.origin.unwrap_or_default());
 
 		value.axis.simplify(&mut joint_builder);
 		value.calibration.simplify(&mut joint_builder);
 		value.dynamics.simplify(&mut joint_builder);
-		value.limit.simplify(&mut joint_builder, false);
+		value
+			.limit
+			.simplify(&mut joint_builder, PrismaticType::IS_CONTINOUS);
 		value.mimic.simplify(&mut joint_builder);
 		value.safety_controller.simplify(&mut joint_builder);
 
 		joint_builder
 	}
 }
```

### Comparing `robot_description_builder-0.0.1/local_dependencies/robot-description-builder/src/joint/smartjointbuilder/smartjointtypes/revolute_joint_type.rs` & `robot_description_builder-0.0.2/local_dependencies/robot-description-builder/src/joint/smartjointbuilder/smartjointtypes/revolute_joint_type.rs`

 * *Files 4% similar despite different names*

```diff
@@ -2,28 +2,30 @@
 
 use crate::{
 	cluster_objects::kinematic_data_tree::KinematicDataTree,
 	joint::JointType,
 	joint::{
 		smartjointbuilder::{
 			smartparams::{
-				smart_joint_datatraits::{self, LimitDataType},
+				smart_joint_datatraits::{self, JointTypeTrait, LimitDataType},
 				smart_joint_specification, WithLimit,
 			},
 			SmartJointBuilder,
 		},
 		BuildJoint, Joint, JointBuilder,
 	},
 	link::Link,
 	ArcLock, WeakLock,
 };
 
 #[derive(Debug, PartialEq, Eq, Clone, Copy, Default)]
 pub struct RevoluteType;
 
+impl_jointtype_traits!(RevoluteType, false);
+
 impl From<RevoluteType> for JointType {
 	fn from(_value: RevoluteType) -> Self {
 		JointType::Revolute
 	}
 }
 
 impl smart_joint_specification::AxisAllowed for RevoluteType {}
@@ -86,14 +88,16 @@
 		let mut joint_builder = JointBuilder::new(value.name, value.joint_type.into());
 
 		joint_builder.with_origin(value.origin.unwrap_or_default());
 
 		value.axis.simplify(&mut joint_builder);
 		value.calibration.simplify(&mut joint_builder);
 		value.dynamics.simplify(&mut joint_builder);
-		value.limit.simplify(&mut joint_builder, false);
+		value
+			.limit
+			.simplify(&mut joint_builder, RevoluteType::IS_CONTINOUS);
 		value.mimic.simplify(&mut joint_builder);
 		value.safety_controller.simplify(&mut joint_builder);
 
 		joint_builder
 	}
 }
```

### Comparing `robot_description_builder-0.0.1/local_dependencies/robot-description-builder/src/joint/smartjointbuilder/smartparams/axis.rs` & `robot_description_builder-0.0.2/local_dependencies/robot-description-builder/src/joint/smartjointbuilder/smartparams/axis.rs`

 * *Files 22% similar despite different names*

```diff
@@ -41,17 +41,23 @@
 			calibration: self.calibration,
 			dynamics: self.dynamics,
 			limit: self.limit,
 			mimic: self.mimic,
 			safety_controller: self.safety_controller,
 		}
 	}
+}
 
-	#[deprecated]
-	/// TODO: Maybe Deprecate
-	pub fn set_axis(
-		self,
-		axis: (f32, f32, f32),
-	) -> SmartJointBuilder<Type, WithAxis, Calibration, Dynamics, Limit, Mimic, SafetyController> {
-		self.with_axis(axis)
+impl<Type, Calibration, Dynamics, Limit, Mimic, SafetyController>
+	SmartJointBuilder<Type, WithAxis, Calibration, Dynamics, Limit, Mimic, SafetyController>
+where
+	Type: AxisAllowed,
+	Calibration: smart_joint_datatraits::CalibrationDataType,
+	Dynamics: smart_joint_datatraits::DynamicsDataType,
+	Limit: smart_joint_datatraits::LimitDataType,
+	Mimic: smart_joint_datatraits::MimicDataType,
+	SafetyController: smart_joint_datatraits::SafetyControllerDataType,
+{
+	pub fn axis(&self) -> (f32, f32, f32) {
+		(self.axis.0, self.axis.1, self.axis.2)
 	}
 }
```

### Comparing `robot_description_builder-0.0.1/local_dependencies/robot-description-builder/src/joint/smartjointbuilder/smartparams/calibration.rs` & `robot_description_builder-0.0.2/local_dependencies/robot-description-builder/src/joint/smartjointbuilder/smartparams/calibration.rs`

 * *Files 4% similar despite different names*

```diff
@@ -69,12 +69,20 @@
 	SafetyController: smart_joint_datatraits::SafetyControllerDataType,
 {
 	pub fn set_rising_calibration(mut self, rising: f32) -> Self {
 		self.calibration.rising = Some(rising);
 		self
 	}
 
+	pub fn rising_calibration(&self) -> Option<f32> {
+		self.calibration.rising
+	}
+
 	pub fn set_falling_calibration(mut self, falling: f32) -> Self {
 		self.calibration.falling = Some(falling);
 		self
 	}
+
+	pub fn falling_calibration(&self) -> Option<f32> {
+		self.calibration.falling
+	}
 }
```

### Comparing `robot_description_builder-0.0.1/local_dependencies/robot-description-builder/src/joint/smartjointbuilder/smartparams/dynamics.rs` & `robot_description_builder-0.0.2/local_dependencies/robot-description-builder/src/joint/smartjointbuilder/smartparams/dynamics.rs`

 * *Files 13% similar despite different names*

```diff
@@ -69,12 +69,20 @@
 	SafetyController: smart_joint_datatraits::SafetyControllerDataType,
 {
 	pub fn set_damping(mut self, damping: f32) -> Self {
 		self.dynamics.damping = Some(damping);
 		self
 	}
 
+	pub fn damping(&self) -> Option<f32> {
+		self.dynamics.damping
+	}
+
 	pub fn set_friction(mut self, friction: f32) -> Self {
 		self.dynamics.friction = Some(friction);
 		self
 	}
+
+	pub fn friction(&self) -> Option<f32> {
+		self.dynamics.friction
+	}
 }
```

### Comparing `robot_description_builder-0.0.1/local_dependencies/robot-description-builder/src/joint/smartjointbuilder/smartparams/limit.rs` & `robot_description_builder-0.0.2/local_dependencies/robot-description-builder/src/joint/smartjointbuilder/smartparams/mimic.rs`

 * *Files 21% similar despite different names*

```diff
@@ -1,119 +1,100 @@
 use crate::joint::{
 	joint_data,
 	jointbuilder::JointBuilder,
 	smartjointbuilder::{smart_joint_datatraits, SmartJointBuilder},
 };
 
-/// TODO: Maybe add a continous lockout thing
-pub trait LimitAllowed {}
+pub trait MimicAllowed {}
 
 #[derive(Debug, Default, Clone)]
-pub struct NoLimit;
-impl smart_joint_datatraits::LimitDataType for NoLimit {}
+pub struct NoMimic;
+impl smart_joint_datatraits::MimicDataType for NoMimic {}
 
+///  (optional) (New with ROS Groovy. See issue)
+///
+/// This tag is used to specify that the defined joint mimics another existing joint. The value of this joint can be computed as value = multiplier * other_joint_value + offset.
+/// TODO: Write better docs
 #[derive(Debug, Default, Clone)]
-pub struct WithLimit {
-	/// An attribute specifying the lower joint limit (in radians for revolute joints, in metres for prismatic joints). Omit if joint is continuous.
-	lower: Option<f32>,
-	/// An attribute specifying the upper joint limit (in radians for revolute joints, in metres for prismatic joints). Omit if joint is continuous.
-	upper: Option<f32>,
-	/// An attribute for enforcing the maximum joint effort (|applied effort| < |effort|).
-	effort: f32,
-	/// An attribute for enforcing the maximum joint velocity (in radians per second [rad/s] for revolute joints, in metres per second [m/s] for prismatic joints).
-	velocity: f32,
+pub struct WithMimic {
+	/// This specifies the name of the joint to mimic.
+	joint_name: String,
+	/// Specifies the multiplicative factor in the formula above.
+	multiplier: Option<f32>,
+	/// Specifies the offset to add in the formula above. Defaults to 0 (radians for revolute joints, meters for prismatic joints)
+	offset: Option<f32>,
 }
 
-impl From<WithLimit> for joint_data::LimitData {
-	fn from(value: WithLimit) -> Self {
+impl From<WithMimic> for joint_data::MimicBuilderData {
+	fn from(value: WithMimic) -> Self {
 		Self {
-			lower: value.lower,
-			upper: value.upper,
-			effort: value.effort,
-			velocity: value.velocity,
+			joint_name: value.joint_name,
+			multiplier: value.multiplier,
+			offset: value.offset,
 		}
 	}
 }
 
-impl smart_joint_datatraits::LimitDataType for WithLimit {
-	fn simplify(&self, joint_builder: &mut JointBuilder, is_continous: bool) {
-		joint_builder.with_limit_data(joint_data::LimitData {
-			lower: match is_continous {
-				true => None,
-				false => self.lower,
-			},
-			upper: match is_continous {
-				true => None,
-				false => self.upper,
-			},
-			effort: self.effort,
-			velocity: self.velocity,
-		})
+impl smart_joint_datatraits::MimicDataType for WithMimic {
+	fn simplify(&self, joint_builder: &mut JointBuilder) {
+		joint_builder.with_mimic_data(self.clone().into())
 	}
 }
 
-impl<Type, Axis, Calibration, Dynamics, Mimic, SafetyController>
-	SmartJointBuilder<Type, Axis, Calibration, Dynamics, NoLimit, Mimic, SafetyController>
+impl<Type, Axis, Calibration, Dynamics, Limit, SafetyController>
+	SmartJointBuilder<Type, Axis, Calibration, Dynamics, Limit, NoMimic, SafetyController>
 where
-	Type: LimitAllowed,
+	Type: MimicAllowed,
 	Axis: smart_joint_datatraits::AxisDataType,
 	Calibration: smart_joint_datatraits::CalibrationDataType,
 	Dynamics: smart_joint_datatraits::DynamicsDataType,
-	Mimic: smart_joint_datatraits::MimicDataType,
+	Limit: smart_joint_datatraits::LimitDataType,
 	SafetyController: smart_joint_datatraits::SafetyControllerDataType,
 {
-	pub fn with_limit(
+	pub fn with_mimic(
 		self,
-		effort: f32,
-		velocity: f32,
-	) -> SmartJointBuilder<Type, Axis, Calibration, Dynamics, WithLimit, Mimic, SafetyController> {
+		mimiced_joint_name: impl Into<String>,
+	) -> SmartJointBuilder<Type, Axis, Calibration, Dynamics, Limit, WithMimic, SafetyController> {
 		SmartJointBuilder {
 			name: self.name,
 			joint_type: self.joint_type,
 			origin: self.origin,
+
 			axis: self.axis,
 			calibration: self.calibration,
 			dynamics: self.dynamics,
-			limit: WithLimit {
-				lower: None,
-				upper: None,
-				effort,
-				velocity,
+			limit: self.limit,
+			mimic: WithMimic {
+				joint_name: mimiced_joint_name.into(),
+				..Default::default()
 			},
-			mimic: self.mimic,
 			safety_controller: self.safety_controller,
 		}
 	}
 }
 
-impl<Type, Axis, Calibration, Dynamics, Mimic, SafetyController>
-	SmartJointBuilder<Type, Axis, Calibration, Dynamics, WithLimit, Mimic, SafetyController>
+impl<Type, Axis, Calibration, Dynamics, Limit, SafetyController>
+	SmartJointBuilder<Type, Axis, Calibration, Dynamics, Limit, WithMimic, SafetyController>
 where
-	Type: LimitAllowed,
+	Type: MimicAllowed,
 	Axis: smart_joint_datatraits::AxisDataType,
 	Calibration: smart_joint_datatraits::CalibrationDataType,
 	Dynamics: smart_joint_datatraits::DynamicsDataType,
-	Mimic: smart_joint_datatraits::MimicDataType,
+	Limit: smart_joint_datatraits::LimitDataType,
 	SafetyController: smart_joint_datatraits::SafetyControllerDataType,
 {
-	pub fn set_effort(mut self, effort: f32) -> Self {
-		self.limit.effort = effort;
-		self
-	}
-
-	pub fn set_velocity(mut self, velocity: f32) -> Self {
-		self.limit.velocity = velocity;
+	pub fn set_mimiced_joint_name(mut self, mimiced_joint_name: impl Into<String>) -> Self {
+		self.mimic.joint_name = mimiced_joint_name.into();
 		self
 	}
 
-	/// TODO: maybe restrict
-	pub fn set_upper_limit(mut self, upper_limit: f32) -> Self {
-		self.limit.upper = Some(upper_limit);
+	pub fn set_mimic_multiplier(mut self, multiplier: f32) -> Self {
+		self.mimic.multiplier = Some(multiplier);
 		self
 	}
 
-	/// TODO: maybe restrict
-	pub fn set_lower_limit(mut self, lower_limit: f32) -> Self {
-		self.limit.lower = Some(lower_limit);
+	/// Specifies the offset to add in the formula above. Defaults to 0 (radians for revolute joints, meters for prismatic joints)
+	pub fn set_mimic_offset(mut self, offset: f32) -> Self {
+		self.mimic.offset = Some(offset);
 		self
 	}
 }
```

### Comparing `robot_description_builder-0.0.1/local_dependencies/robot-description-builder/src/joint/smartjointbuilder/smartparams/safety_controller.rs` & `robot_description_builder-0.0.2/local_dependencies/robot-description-builder/src/joint/smartjointbuilder/smartparams/limit.rs`

 * *Files 14% similar despite different names*

```diff
@@ -1,114 +1,136 @@
 use crate::joint::{
 	joint_data,
 	jointbuilder::JointBuilder,
 	smartjointbuilder::{smart_joint_datatraits, SmartJointBuilder},
 };
 
-pub trait SafetyControllerAllowed {}
+/// TODO: Maybe add a continous lockout thing
+pub trait LimitAllowed {}
 
 #[derive(Debug, Default, Clone)]
-pub struct NoSafetyController;
-impl smart_joint_datatraits::SafetyControllerDataType for NoSafetyController {}
+pub struct NoLimit;
+impl smart_joint_datatraits::LimitDataType for NoLimit {}
 
 #[derive(Debug, Default, Clone)]
-pub struct WithSafetyController {
-	///(optional, defaults to 0)
-	///
-	/// An attribute specifying the lower joint boundary where the safety controller starts limiting the position of the joint. This limit needs to be larger than the lower joint limit (see above). See See safety limits for more details.
-	/// TODO: FIX DOCUMENTATION
-	soft_lower_limit: Option<f32>,
-	/// (optional, defaults to 0)
-	///
-	/// An attribute specifying the upper joint boundary where the safety controller starts limiting the position of the joint. This limit needs to be smaller than the upper joint limit (see above). See See safety limits for more details.
-	/// TODO: FIX DOCUMENTATION
-	soft_upper_limit: Option<f32>,
-	///  (optional, defaults to 0)
-	///
-	/// An attribute specifying the relation between position and velocity limits. See See safety limits for more details.
-	/// TODO: FIX DOCUMENTATION
-	k_position: Option<f32>,
-	/// An attribute specifying the relation between effort and velocity limits. See See safety limits for more details.
-	k_velocity: f32,
+pub struct WithLimit {
+	/// An attribute specifying the lower joint limit (in radians for revolute joints, in metres for prismatic joints). Omit if joint is continuous.
+	lower: Option<f32>,
+	/// An attribute specifying the upper joint limit (in radians for revolute joints, in metres for prismatic joints). Omit if joint is continuous.
+	upper: Option<f32>,
+	/// An attribute for enforcing the maximum joint effort (|applied effort| < |effort|).
+	effort: f32,
+	/// An attribute for enforcing the maximum joint velocity (in radians per second [rad/s] for revolute joints, in metres per second [m/s] for prismatic joints).
+	velocity: f32,
 }
 
-impl From<WithSafetyController> for joint_data::SafetyControllerData {
-	fn from(value: WithSafetyController) -> Self {
+impl From<WithLimit> for joint_data::LimitData {
+	fn from(value: WithLimit) -> Self {
 		Self {
-			soft_lower_limit: value.soft_lower_limit,
-			soft_upper_limit: value.soft_upper_limit,
-			k_position: value.k_position,
-			k_velocity: value.k_velocity,
+			lower: value.lower,
+			upper: value.upper,
+			effort: value.effort,
+			velocity: value.velocity,
 		}
 	}
 }
 
-impl smart_joint_datatraits::SafetyControllerDataType for WithSafetyController {
-	fn simplify(&self, joint_builder: &mut JointBuilder) {
-		joint_builder.with_safety_controller(self.clone().into());
+impl smart_joint_datatraits::LimitDataType for WithLimit {
+	fn simplify(&self, joint_builder: &mut JointBuilder, is_continous: bool) {
+		joint_builder.with_limit_data(joint_data::LimitData {
+			lower: match is_continous {
+				true => None,
+				false => self.lower,
+			},
+			upper: match is_continous {
+				true => None,
+				false => self.upper,
+			},
+			effort: self.effort,
+			velocity: self.velocity,
+		})
 	}
 }
 
-impl<Type, Axis, Calibration, Dynamics, Limit, Mimic>
-	SmartJointBuilder<Type, Axis, Calibration, Dynamics, Limit, Mimic, NoSafetyController>
+impl<Type, Axis, Calibration, Dynamics, Mimic, SafetyController>
+	SmartJointBuilder<Type, Axis, Calibration, Dynamics, NoLimit, Mimic, SafetyController>
 where
-	Type: SafetyControllerAllowed,
+	Type: LimitAllowed,
 	Axis: smart_joint_datatraits::AxisDataType,
 	Calibration: smart_joint_datatraits::CalibrationDataType,
 	Dynamics: smart_joint_datatraits::DynamicsDataType,
-	Limit: smart_joint_datatraits::LimitDataType,
 	Mimic: smart_joint_datatraits::MimicDataType,
+	SafetyController: smart_joint_datatraits::SafetyControllerDataType,
 {
-	pub fn with_safety_controller(
+	pub fn with_limit(
 		self,
-		k_velocity: f32,
-	) -> SmartJointBuilder<Type, Axis, Calibration, Dynamics, Limit, Mimic, WithSafetyController> {
+		effort: f32,
+		velocity: f32,
+	) -> SmartJointBuilder<Type, Axis, Calibration, Dynamics, WithLimit, Mimic, SafetyController> {
 		SmartJointBuilder {
 			name: self.name,
 			joint_type: self.joint_type,
 			origin: self.origin,
-
 			axis: self.axis,
 			calibration: self.calibration,
 			dynamics: self.dynamics,
-			limit: self.limit,
-			mimic: self.mimic,
-			safety_controller: WithSafetyController {
-				k_velocity,
-				..Default::default()
+			limit: WithLimit {
+				lower: None,
+				upper: None,
+				effort,
+				velocity,
 			},
+			mimic: self.mimic,
+			safety_controller: self.safety_controller,
 		}
 	}
 }
 
-impl<Type, Axis, Calibration, Dynamics, Limit, Mimic>
-	SmartJointBuilder<Type, Axis, Calibration, Dynamics, Limit, Mimic, WithSafetyController>
+impl<Type, Axis, Calibration, Dynamics, Mimic, SafetyController>
+	SmartJointBuilder<Type, Axis, Calibration, Dynamics, WithLimit, Mimic, SafetyController>
 where
-	Type: SafetyControllerAllowed,
+	Type: LimitAllowed,
 	Axis: smart_joint_datatraits::AxisDataType,
 	Calibration: smart_joint_datatraits::CalibrationDataType,
 	Dynamics: smart_joint_datatraits::DynamicsDataType,
-	Limit: smart_joint_datatraits::LimitDataType,
 	Mimic: smart_joint_datatraits::MimicDataType,
+	SafetyController: smart_joint_datatraits::SafetyControllerDataType,
 {
-	/// TODO: Add check?
-	pub fn set_soft_lower_limit(mut self, soft_lower_limit: f32) -> Self {
-		self.safety_controller.soft_lower_limit = Some(soft_lower_limit);
+	pub fn set_effort(mut self, effort: f32) -> Self {
+		self.limit.effort = effort;
 		self
 	}
 
-	/// TODO: Add check?
-	pub fn set_soft_upper_limit(mut self, soft_upper_limit: f32) -> Self {
-		self.safety_controller.soft_upper_limit = Some(soft_upper_limit);
+	pub fn effort(&self) -> f32 {
+		self.limit.effort
+	}
+
+	pub fn set_velocity(mut self, velocity: f32) -> Self {
+		self.limit.velocity = velocity;
 		self
 	}
 
-	pub fn set_k_position(mut self, k_position: f32) -> Self {
-		self.safety_controller.k_position = Some(k_position);
+	pub fn velocity(&self) -> f32 {
+		self.limit.velocity
+	}
+}
+
+impl<Type, Axis, Calibration, Dynamics, Mimic, SafetyController>
+	SmartJointBuilder<Type, Axis, Calibration, Dynamics, WithLimit, Mimic, SafetyController>
+where
+	Type: LimitAllowed + smart_joint_datatraits::SmartJointTypeTrait<false>,
+	Axis: smart_joint_datatraits::AxisDataType,
+	Calibration: smart_joint_datatraits::CalibrationDataType,
+	Dynamics: smart_joint_datatraits::DynamicsDataType,
+	Mimic: smart_joint_datatraits::MimicDataType,
+	SafetyController: smart_joint_datatraits::SafetyControllerDataType,
+{
+	pub fn set_upper_limit(mut self, upper_limit: f32) -> Self {
+		self.limit.upper = Some(upper_limit);
 		self
 	}
 
-	pub fn set_k_velocity(mut self, k_velocity: f32) -> Self {
-		self.safety_controller.k_velocity = k_velocity;
+	pub fn set_lower_limit(mut self, lower_limit: f32) -> Self {
+		self.limit.lower = Some(lower_limit);
 		self
 	}
 }
```

### Comparing `robot_description_builder-0.0.1/local_dependencies/robot-description-builder/src/joint/smartjointbuilder/smartparams.rs` & `robot_description_builder-0.0.2/local_dependencies/robot-description-builder/src/joint/smartjointbuilder/smartparams.rs`

 * *Files 3% similar despite different names*

```diff
@@ -17,14 +17,16 @@
 		axis::AxisAllowed, calibration::CalibrationAllowed, dynamics::DynamicsAllowed,
 		limit::LimitAllowed, mimic::MimicAllowed, safety_controller::SafetyControllerAllowed,
 	};
 }
 
 #[allow(unused_variables)]
 pub(crate) mod smart_joint_datatraits {
+	pub use super::super::smartjointtypes::{JointTypeTrait, SmartJointTypeTrait};
+
 	pub trait AxisDataType {
 		fn simplify(&self, joint_builder: &mut crate::joint::jointbuilder::JointBuilder) {}
 	}
 	pub trait CalibrationDataType {
 		fn simplify(&self, joint_builder: &mut crate::joint::jointbuilder::JointBuilder) {}
 	}
 	pub trait DynamicsDataType {
```

### Comparing `robot_description_builder-0.0.1/local_dependencies/robot-description-builder/src/joint/smartjointbuilder.rs` & `robot_description_builder-0.0.2/local_dependencies/robot-description-builder/src/joint/smartjointbuilder.rs`

 * *Files 14% similar despite different names*

```diff
@@ -1,20 +1,19 @@
 mod smartjointtypes;
 
 pub mod smartparams;
-pub use smartjointtypes::{FixedType, NoType, RevoluteType};
+pub use smartjointtypes::{
+	ContinuousType, FixedType, FloatingType, NoType, PlanarType, PrismaticType, RevoluteType,
+};
 
-use super::joint_tranform_mode::JointTransformMode;
+use super::{joint_tranform_mode::JointTransformMode, jointbuilder::JointBuilder};
 use crate::{link::LinkShapeData, transform::Transform};
 use smartparams::{NoAxis, NoCalibration, NoDynamics, NoLimit, NoMimic, NoSafetyController};
 
-use self::{
-	smartjointtypes::{ContinuousType, FloatingType, PlanarType, PrismaticType},
-	smartparams::smart_joint_datatraits,
-};
+use self::smartparams::smart_joint_datatraits;
 
 #[derive(Debug, PartialEq, Clone, Default)]
 pub struct SmartJointBuilder<Type, Axis, Calibration, Dynamics, Limit, Mimic, SafetyController>
 where
 	Axis: smart_joint_datatraits::AxisDataType,
 	Calibration: smart_joint_datatraits::CalibrationDataType,
 	Dynamics: smart_joint_datatraits::DynamicsDataType,
@@ -39,14 +38,19 @@
 	Axis: smart_joint_datatraits::AxisDataType,
 	Calibration: smart_joint_datatraits::CalibrationDataType,
 	Dynamics: smart_joint_datatraits::DynamicsDataType,
 	Limit: smart_joint_datatraits::LimitDataType,
 	Mimic: smart_joint_datatraits::MimicDataType,
 	SafetyController: smart_joint_datatraits::SafetyControllerDataType,
 {
+	pub fn rename(mut self, name: impl Into<String>) -> Self {
+		self.name = name.into();
+		self
+	}
+
 	pub fn add_transform(mut self, transform: Transform) -> Self {
 		self.origin = Some(transform.into());
 		self
 	}
 
 	pub fn add_dynamic_transform(mut self, func: fn(LinkShapeData) -> Transform) -> Self {
 		self.origin = Some(func.into());
@@ -72,86 +76,90 @@
 		SmartJointBuilder {
 			name: name.into(),
 			joint_type: NoType,
 			..SmartJointBuilder::default()
 		}
 	}
 
-	/// TODO: Maybe do it like this
-	/// I Like it...
+	/// Creates a new `SmartJointBuilder` with `JointType::Revolute`
 	pub fn new_revolute(
 		name: impl Into<String>,
 	) -> SmartJointBuilder<
 		RevoluteType,
 		NoAxis,
 		NoCalibration,
 		NoDynamics,
 		NoLimit,
 		NoMimic,
 		NoSafetyController,
 	> {
 		Self::new(name).revolute()
 	}
 
+	/// Creates a new `SmartJointBuilder` of type `Continuous`
 	pub fn new_continuous(
 		name: impl Into<String>,
 	) -> SmartJointBuilder<
 		ContinuousType,
 		NoAxis,
 		NoCalibration,
 		NoDynamics,
 		NoLimit,
 		NoMimic,
 		NoSafetyController,
 	> {
 		Self::new(name).continuous()
 	}
 
+	/// Creates a new `SmartJointBuilder` of type `Prismatic`
 	pub fn new_prismatic(
 		name: impl Into<String>,
 	) -> SmartJointBuilder<
 		PrismaticType,
 		NoAxis,
 		NoCalibration,
 		NoDynamics,
 		NoLimit,
 		NoMimic,
 		NoSafetyController,
 	> {
 		Self::new(name).prismatic()
 	}
 
+	/// Creates a new `SmartJointBuilder` of type `Fixed`
 	pub fn new_fixed(
 		name: impl Into<String>,
 	) -> SmartJointBuilder<
 		FixedType,
 		NoAxis,
 		NoCalibration,
 		NoDynamics,
 		NoLimit,
 		NoMimic,
 		NoSafetyController,
 	> {
 		Self::new(name).fixed()
 	}
 
+	/// Creates a new `SmartJointBuilder` of type `Floating`
 	pub fn new_floating(
 		name: impl Into<String>,
 	) -> SmartJointBuilder<
 		FloatingType,
 		NoAxis,
 		NoCalibration,
 		NoDynamics,
 		NoLimit,
 		NoMimic,
 		NoSafetyController,
 	> {
 		Self::new(name).floating()
 	}
 
+	/// Creates a new `SmartJointBuilder` of type `Planar`
 	pub fn new_planar(
 		name: impl Into<String>,
 	) -> SmartJointBuilder<
 		PlanarType,
 		NoAxis,
 		NoCalibration,
 		NoDynamics,
@@ -304,7 +312,33 @@
 			dynamics: self.dynamics,
 			limit: self.limit,
 			mimic: self.mimic,
 			safety_controller: self.safety_controller,
 		}
 	}
 }
+
+#[cfg(feature = "wrapper")]
+impl<Type, Axis, Calibration, Dynamics, Limit, Mimic, SafetyController>
+	SmartJointBuilder<Type, Axis, Calibration, Dynamics, Limit, Mimic, SafetyController>
+where
+	Type: smart_joint_datatraits::JointTypeTrait,
+	Axis: smart_joint_datatraits::AxisDataType,
+	Calibration: smart_joint_datatraits::CalibrationDataType,
+	Dynamics: smart_joint_datatraits::DynamicsDataType,
+	Limit: smart_joint_datatraits::LimitDataType,
+	Mimic: smart_joint_datatraits::MimicDataType,
+	SafetyController: smart_joint_datatraits::SafetyControllerDataType,
+{
+	pub unsafe fn as_simple(&self) -> JointBuilder {
+		let mut joint_builder = JointBuilder::new(self.name.clone(), self.joint_type.as_type());
+
+		self.axis.simplify(&mut joint_builder);
+		self.calibration.simplify(&mut joint_builder);
+		self.dynamics.simplify(&mut joint_builder);
+		self.limit.simplify(&mut joint_builder, Type::IS_CONTINOUS);
+		self.mimic.simplify(&mut joint_builder);
+		self.safety_controller.simplify(&mut joint_builder);
+
+		joint_builder
+	}
+}
```

### Comparing `robot_description_builder-0.0.1/local_dependencies/robot-description-builder/src/joint.rs` & `robot_description_builder-0.0.2/local_dependencies/robot-description-builder/src/joint.rs`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,14 @@
 mod joint_tranform_mode;
 mod jointbuilder;
+
+#[cfg(not(feature = "smart-joint-extension"))]
 mod smartjointbuilder;
+#[cfg(feature = "smart-joint-extension")]
+pub mod smartjointbuilder;
 
 /// TODO: Pub(crate) for now
 /// pub(crate)
 /// PUB FOR NOW FOR DOC TESTS????
 pub mod joint_data;
 
 pub use joint_tranform_mode::JointTransformMode;
@@ -50,15 +54,15 @@
 }
 
 impl Joint {
 	pub fn name(&self) -> &String {
 		&self.name
 	}
 
-	pub fn jointtype(&self) -> JointType {
+	pub fn joint_type(&self) -> JointType {
 		self.joint_type
 	}
 
 	/// Returns a reference to the parent `Link`
 	///
 	/// TODO: ADD EXAMPLE
 	///
@@ -81,14 +85,19 @@
 		&self.child_link
 	}
 
 	pub fn origin(&self) -> &Transform {
 		&self.origin
 	}
 
+	pub fn axis(&self) -> Option<(f32, f32, f32)> {
+		// This is fine since it implements Copy
+		self.axis
+	}
+
 	/// Make a `JointBuilder` to build a 'Clone' of the `Joint`
 	pub fn rebuild(&self) -> JointBuilder {
 		#[cfg(any(feature = "logging", test))]
 		log::info!(target: "JointBuilder","Rebuilding: {}", self.name());
 		JointBuilder {
 			name: self.name.clone(),
 			joint_type: self.joint_type,
@@ -99,15 +108,14 @@
 			limit: self.limit,
 			mimic: self.mimic.clone().map(|mimic| mimic.into()),
 			safety_controller: self.safety_controller,
 			..Default::default()
 		}
 	}
 
-	/// TODO: MAKE A PUBLIC VERSION WHICH RETURNS WRAPPED IN CHAINED
 	pub(crate) fn rebuild_branch_continued(&self) -> JointBuilder {
 		#[cfg(any(feature = "logging", test))]
 		log::info!(target: "JointBuilder","Rebuilding: {}", self.name());
 		JointBuilder {
 			child: Some(self.child_link.read().unwrap().rebuild_branch_continued()), // FIXME: Figure out if unwrap is Ok here?
 			..self.rebuild()
 		}
@@ -129,15 +137,15 @@
 	pub(crate) fn yank(&self) -> JointBuilder {
 		let builder = self.rebuild_branch_continued();
 
 		#[cfg(any(feature = "logging", test))]
 		log::info!("Yanked Joint \"{}\"", self.name());
 
 		self.parent_link()
-			.try_write()
+			.write()
 			.unwrap() // FIXME: UNWRAP NOT OK
 			.joints_mut()
 			.retain(|joint| !Arc::ptr_eq(&self.get_self(), joint));
 
 		*self.tree.upgrade().unwrap().newest_link.write().unwrap() = Weak::clone(&self.parent_link);
 
 		builder
@@ -166,15 +174,15 @@
 			.create_element("joint")
 			.with_attribute(Attribute {
 				key: QName(b"name"),
 				value: self.name().display().as_bytes().into(),
 			})
 			.with_attribute(Attribute {
 				key: QName(b"type"),
-				value: self.jointtype().into(),
+				value: self.joint_type().into(),
 			});
 
 		element.write_inner_content(|writer| {
 			let origin = self.origin();
 			if origin.contains_some() {
 				origin.to_urdf(writer, urdf_config)?;
 			}
@@ -206,14 +214,15 @@
 						.display()
 						.as_bytes()
 						.into(),
 				})
 				.write_empty()?;
 
 			if let Some((x, y, z)) = &self.axis {
+				// TODO: Fix '<axis xyz="-0 -0 -1"/>' after mirror.
 				writer
 					.create_element("axis")
 					.with_attribute(Attribute {
 						key: QName(b"xyz"),
 						value: format!("{} {} {}", x, y, z).as_bytes().into(),
 					})
 					.write_empty()?;
@@ -242,24 +251,31 @@
 			.read()
 			.unwrap() // FIXME: Is unwrap Ok HEre?
 			.to_urdf(writer, urdf_config)?;
 		Ok(())
 	}
 }
 
-/// TODO: Are all fields covered?
+/// TODO: Maybe remove some fields from check, since it will always match if name and tree are true
 impl PartialEq for Joint {
 	fn eq(&self, other: &Self) -> bool {
 		Weak::ptr_eq(&self.me, &other.me)
 			&& self.name == other.name
 			&& Weak::ptr_eq(&self.tree, &other.tree)
 			&& Weak::ptr_eq(&self.parent_link, &other.parent_link)
 			&& Arc::ptr_eq(&self.child_link, &other.child_link)
 			&& self.joint_type == other.joint_type
 			&& self.origin == other.origin
+			&& self.axis() == other.axis()
+			&& self.calibration == other.calibration
+			&& self.dynamics == other.dynamics
+			&& self.limit == other.limit
+			&& self.mimic == other.mimic
+			&& self.safety_controller == other.safety_controller
+		// `self.me` field is not covered however if they are on the same tree it is impossible to not match `self.me` while matching all the other fields
 	}
 }
 
 /// TODO: Might add data of specif joint type to Struct Spaces.
 #[derive(Debug, PartialEq, Eq, Clone, Copy, Default)]
 pub enum JointType {
 	/// TODO: TEMP DEFAULT
@@ -417,15 +433,14 @@
 					)],
 					..Default::default()
 				}),
 				..Default::default() // TODO: Decide if this is Ok to do in a test
 			}
 		);
 
-		// todo!("FINISH TEST 'lib::joint::test::yank_simple'")
 		// TODO: Maybe the test is to simple
 	}
 
 	#[test]
 	fn yank_less_simple() {
 		let tree = {
 			let material_red = MaterialDescriptor::new_color(1., 0., 0., 1.).named("Red");
```

### Comparing `robot_description_builder-0.0.1/local_dependencies/robot-description-builder/src/lib.rs` & `robot_description_builder-0.0.2/local_dependencies/robot-description-builder/src/lib.rs`

 * *Files 21% similar despite different names*

```diff
@@ -14,27 +14,53 @@
 pub use chained::Chained;
 pub use cluster_objects::{KinematicInterface, KinematicTree, Robot};
 pub use joint::{joint_data, Joint, JointBuilder, JointType, SmartJointBuilder};
 pub use link::{helper_functions, link_data, Link};
 pub use transform::{MirrorAxis, Transform};
 
 pub mod linkbuilding {
-	use super::link;
-	pub use link::builder::*;
+	pub use super::link::builder::*;
 }
 
 /// TODO: Docs
 pub mod prelude {
 	pub use super::cluster_objects::KinematicInterface;
 	pub use super::identifiers::GroupIDChanger;
 	// TODO: maybe add builders to prelude?
 	// pub use joint::{SmartJointBuilder};
 	// pub use material::MaterialDescriptor;
 }
 
+/// TODO: Docs
+
+pub mod errors {
+	pub use super::cluster_objects::kinematic_data_errors::{
+		AddJointError, AddLinkError, AddMaterialError, AddTransmissionError,
+	};
+	pub use super::identifiers::GroupIDError;
+}
+
+#[cfg(feature = "wrapper")]
+pub mod reexport {
+	pub use nalgebra;
+	#[cfg(feature = "xml")]
+	pub use quick_xml;
+}
+
+#[cfg(feature = "smart-joint-extension")]
+pub mod smart_joint_extension {
+	pub mod types {
+		pub use crate::joint::smartjointbuilder::{
+			ContinuousType, FixedType, FloatingType, NoType, PlanarType, PrismaticType,
+			RevoluteType,
+		};
+	}
+	pub use super::joint::smartjointbuilder::smartparams;
+}
+
 #[cfg(test)]
 mod tests {
 	// #[test]
 	// fn it_works() {
 	// 	let result = add(2, 2);
 	// 	assert_eq!(result, 4);
 	// }
```

### Comparing `robot_description_builder-0.0.1/local_dependencies/robot-description-builder/src/link/builder/collision_builder.rs` & `robot_description_builder-0.0.2/local_dependencies/robot-description-builder/src/link/builder/collision_builder.rs`

 * *Files 1% similar despite different names*

```diff
@@ -63,20 +63,20 @@
 		}
 	}
 }
 
 impl Mirror for CollisionBuilder {
 	fn mirrored(&self, mirror_matrix: &Matrix3<f32>) -> Self {
 		Self {
-			name: self.name.as_ref().map(Clone::clone), // FIXME: NAME
+			name: self.name.as_ref().cloned(), // FIXME: NAME
 			origin: self
 				.origin
 				.as_ref()
 				.map(|transform| transform.mirrored(mirror_matrix)),
-			geometry: self.geometry.boxed_mirrored(mirror_matrix), // TODO: this only works on non-chiral geometries, non chiral meshes could maybe be scaled to neg
+			geometry: self.geometry.boxed_mirrored(mirror_matrix),
 		}
 	}
 }
 
 /// Non-builder methods
 impl CollisionBuilder {
 	pub fn name(&self) -> Option<&String> {
```

### Comparing `robot_description_builder-0.0.1/local_dependencies/robot-description-builder/src/link/builder/linkbuilder.rs` & `robot_description_builder-0.0.2/local_dependencies/robot-description-builder/src/link/builder/linkbuilder.rs`

 * *Files 3% similar despite different names*

```diff
@@ -14,14 +14,16 @@
 };
 
 #[derive(Debug, PartialEq, Clone, Default)]
 pub struct LinkBuilder {
 	// All fields are pub(crate) so I can struct initialize in rebuild
 	pub(crate) name: String,
 	/// TODO: Figure out if we make this immutable on a `Link` and only allow editting throug the builder.
+	///
+	/// TODO: Change name or change name of `colliders` make them consitent
 	pub(crate) visual_builders: Vec<VisualBuilder>,
 	pub(crate) colliders: Vec<CollisionBuilder>,
 	/// TODO: Calulate InertialData?
 	pub(crate) intertial: Option<link_data::InertialData>,
 	pub(crate) joints: Vec<JointBuilder>,
 }
 
@@ -42,20 +44,32 @@
 	/// TODO: Not really sure if this is the way... but it is how clap does it.
 	pub fn add_collider(mut self, collider: CollisionBuilder) -> Self {
 		self.colliders.push(collider);
 		self
 	}
 
 	/// TODO: Naming not inline with convention
-	pub fn intertial(mut self, inertial: link_data::InertialData) -> Self {
+	/// Not happy with the added `add_` but otherwise name colliding with getter
+	pub fn add_intertial(mut self, inertial: link_data::InertialData) -> Self {
 		self.intertial = Some(inertial);
 		self
 	}
 
-	// ===== NON BUILDER METHODS =====
+	/// FIXME: This is temporary, since BuildLink is now a private trait
+	/// I think this might be fine
+	pub fn build_tree(self) -> KinematicTree {
+		BuildLink::build_tree(self)
+	}
+}
+
+/// Non-builder methods
+impl LinkBuilder {
+	pub fn name(&self) -> &String {
+		&self.name
+	}
 
 	pub fn visuals(&self) -> &Vec<VisualBuilder> {
 		&self.visual_builders
 	}
 
 	pub fn visuals_mut(&mut self) -> &mut Vec<VisualBuilder> {
 		&mut self.visual_builders
@@ -69,22 +83,16 @@
 		&mut self.colliders
 	}
 
 	pub fn joints(&self) -> &Vec<JointBuilder> {
 		&self.joints
 	}
 
-	// pub(crate) fn build(self, tree: ArcLock<KinematicTreeData>) -> ArcLock<Link> {
-	//     // Not sure How i wanna do this yet,
-	//     // Maybe with colliders and visuals, stacking and calculating the always calculating the endpoint or not?
-	// }
-
-	/// FIXME: This is temporary, since BuildLink is now a private trait
-	pub fn build_tree(self) -> KinematicTree {
-		BuildLink::build_tree(self)
+	pub fn inertial(&self) -> Option<&link_data::InertialData> {
+		self.intertial.as_ref()
 	}
 }
 
 impl Mirror for LinkBuilder {
 	fn mirrored(&self, mirror_matrix: &Matrix3<f32>) -> Self {
 		Self {
 			name: self.name.clone(), // TODO: rename mirrored
@@ -131,15 +139,14 @@
 				)
 				.unwrap(),
 				colliders: self
 					.colliders
 					.into_iter()
 					.map(|collision_builder| collision_builder.build())
 					.collect(),
-				end_point: None, //TODO:
 				me: Weak::clone(me),
 			})
 		})
 	}
 
 	fn start_building_chain(self, tree: &Weak<KinematicDataTree>) -> ArcLock<Link> {
 		let joint_builders = self.joints.clone();
@@ -184,15 +191,14 @@
 				)
 				.unwrap(), // UNWRAP NOT OK
 				colliders: self
 					.colliders
 					.into_iter()
 					.map(|collider_builder| collider_builder.build())
 					.collect(),
-				end_point: None, // FIXME: Fix this
 				me: Weak::clone(me),
 			})
 		})
 	}
 
 	fn get_shape_data(&self) -> LinkShapeData {
 		LinkShapeData::new(
```

### Comparing `robot_description_builder-0.0.1/local_dependencies/robot-description-builder/src/link/builder/visual_builder.rs` & `robot_description_builder-0.0.2/local_dependencies/robot-description-builder/src/link/builder/visual_builder.rs`

 * *Files 1% similar despite different names*

```diff
@@ -58,15 +58,15 @@
 	}
 
 	pub fn materialized(mut self, material_description: MaterialDescriptor) -> Self {
 		self.material_description = Some(material_description);
 		self
 	}
 
-	/// FIXME: Propper Error
+	/// FIXME: Propper Error, Which error?
 	pub(crate) fn build(self) -> Result<Visual, String> {
 		let material = self
 			.material_description
 			.map(|description| description.build());
 
 		Ok(Visual {
 			name: self.name,
@@ -83,20 +83,20 @@
 		}
 	}
 }
 
 impl Mirror for VisualBuilder {
 	fn mirrored(&self, mirror_matrix: &Matrix3<f32>) -> Self {
 		Self {
-			name: self.name.as_ref().map(Clone::clone), // TODO: Fix
+			name: self.name.as_ref().cloned(), // TODO: Fix
 			origin: self
 				.origin
 				.as_ref()
 				.map(|transform| transform.mirrored(mirror_matrix)),
-			geometry: self.geometry.boxed_mirrored(mirror_matrix), // TODO: this only works on non-chiral geometries, FIX described in `CollisionBuilder`
+			geometry: self.geometry.boxed_mirrored(mirror_matrix),
 			material_description: self.material_description.clone(),
 		}
 	}
 }
 
 /// Non-builder methods
 impl VisualBuilder {
```

### Comparing `robot_description_builder-0.0.1/local_dependencies/robot-description-builder/src/link/builder.rs` & `robot_description_builder-0.0.2/local_dependencies/robot-description-builder/src/link/builder.rs`

 * *Files identical despite different names*

### Comparing `robot_description_builder-0.0.1/local_dependencies/robot-description-builder/src/link/collision.rs` & `robot_description_builder-0.0.2/local_dependencies/robot-description-builder/src/link/collision.rs`

 * *Files identical despite different names*

### Comparing `robot_description_builder-0.0.1/local_dependencies/robot-description-builder/src/link/geometry/box_geometry.rs` & `robot_description_builder-0.0.2/local_dependencies/robot-description-builder/src/link/geometry/box_geometry.rs`

 * *Files identical despite different names*

### Comparing `robot_description_builder-0.0.1/local_dependencies/robot-description-builder/src/link/geometry/cylinder_geometry.rs` & `robot_description_builder-0.0.2/local_dependencies/robot-description-builder/src/link/geometry/cylinder_geometry.rs`

 * *Files identical despite different names*

### Comparing `robot_description_builder-0.0.1/local_dependencies/robot-description-builder/src/link/geometry/geometry_shape_data.rs` & `robot_description_builder-0.0.2/local_dependencies/robot-description-builder/src/link/geometry/geometry_shape_data.rs`

 * *Files identical despite different names*

### Comparing `robot_description_builder-0.0.1/local_dependencies/robot-description-builder/src/link/geometry/mesh_geometry.rs` & `robot_description_builder-0.0.2/local_dependencies/robot-description-builder/src/link/geometry/mesh_geometry.rs`

 * *Files identical despite different names*

### Comparing `robot_description_builder-0.0.1/local_dependencies/robot-description-builder/src/link/geometry/sphere_geometry.rs` & `robot_description_builder-0.0.2/local_dependencies/robot-description-builder/src/link/geometry/sphere_geometry.rs`

 * *Files identical despite different names*

### Comparing `robot_description_builder-0.0.1/local_dependencies/robot-description-builder/src/link/geometry.rs` & `robot_description_builder-0.0.2/local_dependencies/robot-description-builder/src/link/geometry.rs`

 * *Files 3% similar despite different names*

```diff
@@ -8,19 +8,22 @@
 pub use box_geometry::BoxGeometry;
 pub use cylinder_geometry::CylinderGeometry;
 pub use mesh_geometry::MeshGeometry;
 pub use sphere_geometry::SphereGeometry;
 
 pub use geometry_shape_data::GeometryShapeData;
 
+// TODO: Maybe only exported for `wrapping` feature
+pub use geometry_shape_data::GeometryShapeContainer;
+
 use std::fmt::Debug;
 
 use crate::transform::Mirror;
 
-use self::geometry_shape_data::GeometryShapeContainer;
+// use self::geometry_shape_data::GeometryShapeContainer;
 
 pub trait BoxedMirror {
 	fn boxed_mirrored(
 		&self,
 		mirror_matrix: &Matrix3<f32>,
 	) -> Box<dyn GeometryInterface + Sync + Send>;
 }
@@ -63,13 +66,12 @@
 		// Should probably just get shape data
 		self.volume() == other.volume()
 			&& self.surface_area() == other.surface_area()
 			&& self.bounding_box() == other.bounding_box()
 	}
 }
 
-// TODO: Is this ever used?
 impl From<&(dyn GeometryInterface + Sync + Send)> for Box<dyn GeometryInterface + Sync + Send> {
 	fn from(value: &(dyn GeometryInterface + Sync + Send)) -> Self {
 		value.boxed_clone()
 	}
 }
```

### Comparing `robot_description_builder-0.0.1/local_dependencies/robot-description-builder/src/link/helper_functions.rs` & `robot_description_builder-0.0.2/local_dependencies/robot-description-builder/src/link/helper_functions.rs`

 * *Files identical despite different names*

### Comparing `robot_description_builder-0.0.1/local_dependencies/robot-description-builder/src/link/inertial.rs` & `robot_description_builder-0.0.2/local_dependencies/robot-description-builder/src/link/inertial.rs`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 use crate::transform::{Mirror, Transform};
 
 #[cfg(feature = "urdf")]
 use crate::to_rdf::to_urdf::ToURDF;
 #[cfg(feature = "xml")]
 use quick_xml::{events::attributes::Attribute, name::QName};
 
-#[derive(Debug, PartialEq, Clone, Default)]
+#[derive(Debug, PartialEq, Clone, Copy, Default)]
 /// TODO: Figure out if things should be private or not?
 pub struct InertialData {
 	pub origin: Option<Transform>,
 	pub mass: f32,
 	pub ixx: f32, // Not the nicesest way of doing this.
 	pub ixy: f32,
 	pub ixz: f32,
@@ -23,15 +23,15 @@
 impl Mirror for InertialData {
 	fn mirrored(&self, mirror_matrix: &Matrix3<f32>) -> Self {
 		Self {
 			origin: self
 				.origin
 				.as_ref()
 				.map(|transform| transform.mirrored(mirror_matrix)),
-			..self.clone()
+			..*self
 		}
 	}
 }
 
 #[cfg(feature = "urdf")]
 impl ToURDF for InertialData {
 	fn to_urdf(
```

### Comparing `robot_description_builder-0.0.1/local_dependencies/robot-description-builder/src/link/link_parent.rs` & `robot_description_builder-0.0.2/local_dependencies/robot-description-builder/src/link/link_parent.rs`

 * *Files identical despite different names*

### Comparing `robot_description_builder-0.0.1/local_dependencies/robot-description-builder/src/link/link_shape_data.rs` & `robot_description_builder-0.0.2/local_dependencies/robot-description-builder/src/link/link_shape_data.rs`

 * *Files identical despite different names*

### Comparing `robot_description_builder-0.0.1/local_dependencies/robot-description-builder/src/link/visual.rs` & `robot_description_builder-0.0.2/local_dependencies/robot-description-builder/src/link/visual.rs`

 * *Files 1% similar despite different names*

```diff
@@ -67,15 +67,15 @@
 	}
 
 	pub fn rebuild(&self) -> VisualBuilder {
 		VisualBuilder {
 			name: self.name.clone(),
 			origin: self.origin,
 			geometry: self.geometry.boxed_clone(),
-			material_description: self.material.as_ref().map(|material| material.rebuild()), // UNWRAP???
+			material_description: self.material.as_ref().map(|material| material.describe()),
 		}
 	}
 
 	pub(crate) fn get_geometry_data(&self) -> GeometryShapeData {
 		GeometryShapeData {
 			origin: self.origin.unwrap_or_default(),
 			geometry: self.geometry.shape_container(),
```

### Comparing `robot_description_builder-0.0.1/local_dependencies/robot-description-builder/src/link.rs` & `robot_description_builder-0.0.2/local_dependencies/robot-description-builder/src/link.rs`

 * *Files 1% similar despite different names*

```diff
@@ -20,23 +20,23 @@
 	pub use crate::link::inertial::InertialData;
 	pub use crate::link::link_parent::LinkParent;
 	pub use crate::link::visual::Visual;
 	pub mod geometry {
 		pub use crate::link::geometry::*;
 	}
 
-	/// TODO: Depricate or Implement?
-	#[derive(Debug, PartialEq, Eq, Clone)]
-	pub enum ConnectionPoint {
-		/// Point at Link connection point (Link Origin without translation)
-		Begin,
-		CenterOfVolume,
-		CenterOfMass,
-		End,
-	}
+	// /// TODO: Depricate or Implement?
+	// #[derive(Debug, PartialEq, Eq, Clone)]
+	// pub enum ConnectionPoint {
+	// 	/// Point at Link connection point (Link Origin without translation)
+	// 	Begin,
+	// 	CenterOfVolume,
+	// 	CenterOfMass,
+	// 	End,
+	// }
 }
 
 use std::sync::{Arc, Weak};
 
 #[cfg(feature = "urdf")]
 use crate::to_rdf::to_urdf::ToURDF;
 use crate::{
@@ -53,24 +53,24 @@
 	transform::Transform,
 	ArcLock, WeakLock,
 };
 
 /// TODO: Make Builder For Link
 #[derive(Debug)]
 pub struct Link {
-	pub(crate) name: String,
+	name: String,
 	pub(crate) tree: Weak<KinematicDataTree>,
 	direct_parent: link_data::LinkParent,
 	child_joints: Vec<ArcLock<Joint>>,
 	inertial: Option<InertialData>,
 	visuals: Vec<link_data::Visual>,
 	colliders: Vec<link_data::Collision>,
-	/// TODO: Maybe array, or thing
-	/// Or calculate when necessary
-	end_point: Option<(f32, f32, f32)>,
+	// /// TODO: Maybe array, or thing
+	// /// Or calculate when necessary
+	// end_point: Option<(f32, f32, f32)>,
 	me: WeakLock<Self>,
 }
 
 impl Link {
 	pub fn builder(name: impl Into<String>) -> LinkBuilder {
 		LinkBuilder::new(name)
 	}
@@ -178,48 +178,47 @@
 		Ok(())
 	}
 
 	pub fn inertial(&self) -> Option<&InertialData> {
 		self.inertial.as_ref()
 	}
 
-	pub fn get_end_point(&self) -> Option<(f32, f32, f32)> {
-		self.end_point
-	}
+	// pub fn get_end_point(&self) -> Option<(f32, f32, f32)> {
+	// 	self.end_point
+	// }
 
 	pub fn visuals(&self) -> &Vec<Visual> {
 		&self.visuals
 	}
 
 	pub(crate) fn visuals_mut(&mut self) -> &mut Vec<Visual> {
 		&mut self.visuals
 	}
 
 	pub fn colliders(&self) -> &Vec<Collision> {
 		&self.colliders
 	}
 
-	/// TODO: EXPAND
 	pub fn rebuild(&self) -> LinkBuilder {
 		LinkBuilder {
 			name: self.name.clone(),
 			visual_builders: self.visuals.iter().map(|visual| visual.rebuild()).collect(),
 			colliders: self
 				.colliders
 				.iter()
 				.map(|collision| collision.rebuild())
 				.collect(),
-			intertial: self.inertial.clone(),
+			intertial: self.inertial,
 			..Default::default()
 		}
 	}
 
 	/// Rebuilds everything below this aswell
 	///
-	/// TODO: FINISH
+	/// TODO: DOCS
 	pub(crate) fn rebuild_branch_continued(&self) -> LinkBuilder {
 		LinkBuilder {
 			joints: self
 				.child_joints
 				.iter()
 				.map(|joint| joint.read().unwrap().rebuild_branch_continued()) // FIXME: Figure out if unwrap is Ok here?
 				.collect(),
@@ -247,15 +246,15 @@
 
 				*self.tree.upgrade().unwrap().newest_link.write().unwrap() =
 					Weak::clone(parent_link);
 
 				parent_link
 					.upgrade()
 					.unwrap() // This unwrap is Ok since the parent_link on a Joint is initialized while adding to the tree.
-					.try_write()
+					.write()
 					.unwrap() //FIXME: Is unwrap Ok here?
 					.joints_mut()
 					.retain(|other_joint| !Arc::ptr_eq(&joint, other_joint));
 			}
 			LinkParent::KinematicTree(_) => {
 				#[cfg(any(feature = "logging", test))]
 				log::trace!("The tree should be dropped, but how?")
```

### Comparing `robot_description_builder-0.0.1/local_dependencies/robot-description-builder/src/material/data.rs` & `robot_description_builder-0.0.2/local_dependencies/robot-description-builder/src/material/data.rs`

 * *Files identical despite different names*

### Comparing `robot_description_builder-0.0.1/local_dependencies/robot-description-builder/src/material/descriptor.rs` & `robot_description_builder-0.0.2/local_dependencies/robot-description-builder/src/material/descriptor.rs`

 * *Files identical despite different names*

### Comparing `robot_description_builder-0.0.1/local_dependencies/robot-description-builder/src/material/stage.rs` & `robot_description_builder-0.0.2/local_dependencies/robot-description-builder/src/material/stage.rs`

 * *Files 10% similar despite different names*

```diff
@@ -33,19 +33,21 @@
 			MaterialStage::PreInit(_) => *self = MaterialStage::Initialized(material_data),
 			MaterialStage::Initialized(data) => {
 				debug_assert!(Arc::ptr_eq(data, &material_data));
 			}
 		}
 	}
 
-	/// TODO: WHAT TO DO WHIT NAME? with regards to convention
-	pub(crate) fn get_data(&self) -> MaterialDataReferenceWrapper {
+	/// Gets the data wrapped in a `MaterialDataReferenceWrapper`
+	///
+	/// TODO: Name could also be `get`
+	pub(crate) fn data(&self) -> MaterialDataReferenceWrapper {
 		match self {
 			MaterialStage::PreInit(data) => data.into(),
-			MaterialStage::Initialized(arc_data) => Arc::clone(arc_data).into(), //Unwrap not Ok
+			MaterialStage::Initialized(arc_data) => Arc::clone(arc_data).into(),
 		}
 	}
 }
 
 #[cfg(feature = "urdf")]
 impl ToURDF for MaterialStage {
 	fn to_urdf(
```

### Comparing `robot_description_builder-0.0.1/local_dependencies/robot-description-builder/src/material.rs` & `robot_description_builder-0.0.2/local_dependencies/robot-description-builder/src/material.rs`

 * *Files 10% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+//! The `Material` System
+//!
 //! TODO: MODULE DOC
 // DOCS TODO:
 //  - Module
 //  - Material
 //  - MaterialDescriptor
 mod descriptor;
 pub(crate) mod stage;
@@ -61,15 +63,17 @@
 	) -> Self {
 		Self(MaterialKind::Named {
 			name: name.into(),
 			data: MaterialStage::Initialized(data),
 		})
 	}
 
-	/// TODO: DOCS
+	/// Register the `Material` in the `KinematicDataTree`.
+	///
+	/// TODO: EXPAND
 	pub(crate) fn initialize(&mut self, tree: &KinematicDataTree) -> Result<(), AddMaterialError> {
 		match &mut self.0 {
 			// An unnamed Material does not have to be initialized.
 			MaterialKind::Unnamed(_) => Ok(()),
 			MaterialKind::Named { name, data } => {
 				let material_data = match data {
 					MaterialStage::PreInit(data) => {
@@ -111,33 +115,43 @@
 				};
 				data.initialize(material_data);
 				Ok(())
 			}
 		}
 	}
 
+	/// The `name` of the `Material` if any.
+	///
+	/// Returns the `Some(name)` for a named [`Material`] and `None` for an unnamed [`Material`].
 	pub fn name(&self) -> Option<&String> {
 		match &self.0 {
 			MaterialKind::Named { name, data: _ } => Some(name),
 			MaterialKind::Unnamed(_) => None,
 		}
 	}
 
+	/// get a refeence to the `MaterialData` as a `MaterialDataReferenceWrapper`
+	///
+	/// TODO: EXPAND
+	/// TODO: Consider removing Wrapper for name of MaterialDataReferenceWrapper.
 	pub fn material_data(&self) -> MaterialDataReferenceWrapper {
 		match &self.0 {
-			MaterialKind::Named { name: _, data } => data.get_data(),
+			MaterialKind::Named { name: _, data } => data.data(),
 			MaterialKind::Unnamed(data) => data.into(),
 		}
 	}
 
-	pub fn rebuild(&self) -> MaterialDescriptor {
-		let builder = MaterialDescriptor::new_data(self.material_data().try_into().unwrap()); //FIXME: Unwrap not OK
+	/// Describes the `Material` to reform a `MaterialDescriptor`.
+	///
+	/// TODO: Expand
+	pub fn describe(&self) -> MaterialDescriptor {
+		let descriptor = MaterialDescriptor::new_data(self.material_data().try_into().unwrap()); //FIXME: Unwrap not OK
 		match &self.0 {
-			MaterialKind::Named { name, data: _ } => builder.named(name),
-			MaterialKind::Unnamed(_) => builder,
+			MaterialKind::Named { name, data: _ } => descriptor.named(name),
+			MaterialKind::Unnamed(_) => descriptor,
 		}
 	}
 }
 
 #[cfg(feature = "urdf")]
 impl ToURDF for Material {
 	fn to_urdf(
@@ -164,14 +178,15 @@
 				element.write_inner_content(|writer| data.to_urdf(writer, urdf_config))?
 			}
 		};
 		Ok(())
 	}
 }
 
+#[cfg(feature = "wrapper")]
 impl From<(String, ArcLock<MaterialData>)> for Material {
 	fn from(value: (String, ArcLock<MaterialData>)) -> Self {
 		let name = value.0;
 		let data = value.1;
 
 		Self::new_named_inited(name, data)
 	}
```

### Comparing `robot_description_builder-0.0.1/local_dependencies/robot-description-builder/src/to_rdf/to_sdf.rs` & `robot_description_builder-0.0.2/local_dependencies/robot-description-builder/src/to_rdf/to_sdf.rs`

 * *Files identical despite different names*

### Comparing `robot_description_builder-0.0.1/local_dependencies/robot-description-builder/src/to_rdf/to_urdf.rs` & `robot_description_builder-0.0.2/local_dependencies/robot-description-builder/src/to_rdf/to_urdf.rs`

 * *Files identical despite different names*

### Comparing `robot_description_builder-0.0.1/local_dependencies/robot-description-builder/src/to_rdf.rs` & `robot_description_builder-0.0.2/local_dependencies/robot-description-builder/src/to_rdf.rs`

 * *Files identical despite different names*

### Comparing `robot_description_builder-0.0.1/local_dependencies/robot-description-builder/src/transform.rs` & `robot_description_builder-0.0.2/local_dependencies/robot-description-builder/src/transform.rs`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 //! INTERNALDOC: This contains module [`Transform`], [`MirrorAxis`] and the core mirror logic.
 // User docs finished
+// TODO: MirrorDocs
 use itertools::Itertools;
 use nalgebra::{vector, Matrix3, Rotation3, Vector3};
 
 #[cfg(feature = "urdf")]
 use crate::to_rdf::to_urdf::ToURDF;
 #[cfg(feature = "xml")]
 use quick_xml::{events::attributes::Attribute, name::QName};
@@ -227,21 +228,34 @@
 			MirrorAxis::Z => (1., 1., -1.),
 		};
 
 		Matrix3::from_diagonal(&Vector3::new(diag.0, diag.1, diag.2))
 	}
 }
 
+/// A mirrorable type
+///
+/// Types implementing `Mirror` are able to be [`mirrored`](Mirror::mirrored), given an `mirror_matrix`.
 pub(crate) trait Mirror {
+	/// Returns a mirrored clone of itself
+	///
+	/// TODO: EXAMPLE
 	fn mirrored(&self, mirror_matrix: &Matrix3<f32>) -> Self;
 }
 
+/// A type which can change the `mirror_matrix` for its children.
+///
+/// TODO: IMPROVE/FINISH DOCS
+///
+/// Types implementing `MirrorUpdater` can be [`mirrored`](Mirror::mirrored). As a result of this mirror the `mirror_matrix` changes.
 pub(crate) trait MirrorUpdater: Sized + Mirror {
+	/// Get the updated `mirror_matrix` which should be used for all children.
 	fn update_mirror_matrix(&self, mirror_matrix: &Matrix3<f32>) -> Matrix3<f32>;
 
+	/// Return a mirrored clone of itself and the updated `mirror_matrix`.
 	fn mirrored_update_matrix(&self, mirror_matrix: &Matrix3<f32>) -> (Self, Matrix3<f32>) {
 		(
 			self.mirrored(mirror_matrix),
 			self.update_mirror_matrix(mirror_matrix),
 		)
 	}
 }
```

### Comparing `robot_description_builder-0.0.1/local_dependencies/robot-description-builder/src/transmission/build_transmission_error.rs` & `robot_description_builder-0.0.2/local_dependencies/robot-description-builder/src/transmission/build_transmission_error.rs`

 * *Files identical despite different names*

### Comparing `robot_description_builder-0.0.1/local_dependencies/robot-description-builder/src/transmission/hardware_interface.rs` & `robot_description_builder-0.0.2/local_dependencies/robot-description-builder/src/transmission/hardware_interface.rs`

 * *Files 7% similar despite different names*

```diff
@@ -7,14 +7,18 @@
 ///
 /// This is really vague and confusion
 ///
 /// <https://docs.ros.org/en/noetic/api/transmission_interface/html/c++/classtransmission__interface_1_1TransmissionInterfaceLoader.html#details>
 /// <https://github.com/ros-controls/ros_control/wiki/hardware_interface#hardware-interfaces>
 ///
 /// TODO: Maybe add other variant with argument
+///
+/// <https://github.com/ros-controls/ros_control/wiki/hardware_interface>
+///
+/// `gazebo_ros_control` does not support multiple HardwareInterfaces for a Joint in one transmission <https://answers.ros.org/question/235040/gazebo_ros_control-lwa4p/>
 #[non_exhaustive]
 #[derive(Debug, PartialEq, Eq, Clone, Copy)]
 pub enum TransmissionHardwareInterface {
 	/// TODO: THIS MIGHT BE A CATEGORY
 	JointCommandInterface,
 	/// TODO: DOCS
 	/// Supported in Gazebo ROS by gazebo_ros_control [Source](https://classic.gazebosim.org/tutorials?tut=ros_control&cat=connect_ros#Defaultgazebo_ros_controlBehavior)
```

### Comparing `robot_description_builder-0.0.1/local_dependencies/robot-description-builder/src/transmission/mod.rs` & `robot_description_builder-0.0.2/local_dependencies/robot-description-builder/src/transmission/mod.rs`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,14 @@
 //! TODO: MODULE DOC
+//! This needs a rewrite, since the system is very different then on first inspection.
+//!
+//! struct Transmission {
+//!     name: String
+//!     data: TransmissionType/dyn impl TransmissionInterface
+//! }
 //!
 
 mod build_transmission_error;
 mod hardware_interface;
 mod transmission_actuator;
 mod transmission_joint;
 mod transmission_type;
@@ -68,18 +74,21 @@
 	impl TransmissionActuatorTrait for WithActuator {
 		fn into_inner(self) -> Vec<super::TransmissionActuator> {
 			self.0
 		}
 	}
 }
 
-use transmission_builder_state::{
-	NoActuator, NoJoints, TransmissionActuatorTrait, TransmissionJointTrait, WithActuator,
-	WithJoints,
-};
+#[cfg(feature = "wrapper")]
+pub use transmission_builder_state::{NoActuator, NoJoints, WithActuator, WithJoints};
+
+#[cfg(not(feature = "wrapper"))]
+use transmission_builder_state::{NoActuator, NoJoints, WithActuator, WithJoints};
+
+use transmission_builder_state::{TransmissionActuatorTrait, TransmissionJointTrait};
 
 #[derive(Debug, PartialEq, Clone)]
 pub struct TransmissionBuilder<Joints, Actuators>
 where
 	Joints: TransmissionJointTrait,
 	Actuators: TransmissionActuatorTrait,
 {
@@ -116,60 +125,15 @@
 		TransmissionBuilder {
 			name: self.name,
 			transmission_type: self.transmission_type,
 			joints: WithJoints(joints),
 			actuators: self.actuators,
 		}
 	}
-}
-
-// impl<Actuator> TransmissionBuilder<NoJoints, Actuator>
-// where
-// 	Actuator: TransmissionActuatorTrait,
-// {
-// 	pub fn add_joint(
-// 		self,
-// 		joint_name: impl Into<String>,
-// 		hardware_interface: TransmissionHardwareInterface,
-// 	) -> TransmissionBuilder<WithJoints, Actuator> {
-// 		TransmissionBuilder {
-// 			name: self.name,
-// 			transmission_type: self.transmission_type,
-// 			joints: WithJoints(vec![TransmissionJointBuilder::new(
-// 				joint_name,
-// 				hardware_interface,
-// 			)]),
-// 			actuators: self.actuators,
-// 		}
-// 	}
-// }
-
-// impl<Actuator> TransmissionBuilder<WithJoints, Actuator>
-// where
-// 	Actuator: TransmissionActuatorTrait,
-// {
-// 	pub fn add_joint(
-// 		mut self,
-// 		joint_name: impl Into<String>,
-// 		hardware_interface: TransmissionHardwareInterface,
-// 	) -> TransmissionBuilder<WithJoints, Actuator> {
-// 		self.joints.0.push(TransmissionJointBuilder::new(
-// 			joint_name,
-// 			hardware_interface,
-// 		));
-
-// 		self
-// 	}
-// }
 
-impl<Joints, Actuators> TransmissionBuilder<Joints, Actuators>
-where
-	Joints: TransmissionJointTrait,
-	Actuators: TransmissionActuatorTrait,
-{
 	pub fn add_actuator(
 		self,
 		transmission_actuator: TransmissionActuator,
 	) -> TransmissionBuilder<Joints, WithActuator> {
 		let mut actuators = self.actuators.into_inner();
 
 		actuators.push(transmission_actuator);
@@ -177,46 +141,60 @@
 		TransmissionBuilder {
 			name: self.name,
 			transmission_type: self.transmission_type,
 			joints: self.joints,
 			actuators: WithActuator(actuators),
 		}
 	}
+
+	/// Gets a reference to the name of the current `TransmissionBuilder`.
+	pub fn name(&self) -> &String {
+		&self.name
+	}
+
+	pub fn transmission_type(&self) -> &TransmissionType {
+		&self.transmission_type
+	}
 }
 
-// impl<Joints> TransmissionBuilder<Joints, NoActuator>
-// where
-// 	Joints: TransmissionJointTrait,
-// {
-// 	pub fn add_actuator(
-// 		self,
-// 		transmission_actuator: TransmissionActuator,
-// 	) -> TransmissionBuilder<Joints, WithActuator> {
-// 		TransmissionBuilder {
-// 			name: self.name,
-// 			transmission_type: self.transmission_type,
-// 			joints: self.joints,
-// 			actuators: WithActuator(vec![transmission_actuator]),
-// 		}
-// 	}
-// }
-
-// impl<Joints> TransmissionBuilder<Joints, WithActuator>
-// where
-// 	Joints: TransmissionJointTrait,
-// {
-// 	pub fn add_actuator(
-// 		mut self,
-// 		transmission_actuator: TransmissionActuator,
-// 	) -> TransmissionBuilder<Joints, WithActuator> {
-// 		self.actuators.0.push(transmission_actuator);
-
-// 		self
-// 	}
-// }
+impl<Actuators> TransmissionBuilder<WithJoints, Actuators>
+where
+	Actuators: TransmissionActuatorTrait,
+{
+	pub fn joints(&self) -> Option<&Vec<TransmissionJointBuilder>> {
+		Some(&self.joints.0)
+	}
+}
+
+impl<Actuators> TransmissionBuilder<NoJoints, Actuators>
+where
+	Actuators: TransmissionActuatorTrait,
+{
+	pub fn joints(&self) -> Option<&Vec<TransmissionJointBuilder>> {
+		None
+	}
+}
+
+impl<Joints> TransmissionBuilder<Joints, WithActuator>
+where
+	Joints: TransmissionJointTrait,
+{
+	pub fn actuators(&self) -> Option<&Vec<TransmissionActuator>> {
+		Some(&self.actuators.0)
+	}
+}
+
+impl<Joints> TransmissionBuilder<Joints, NoActuator>
+where
+	Joints: TransmissionJointTrait,
+{
+	pub fn actuators(&self) -> Option<&Vec<TransmissionActuator>> {
+		None
+	}
+}
 
 impl TransmissionBuilder<WithJoints, WithActuator> {
 	pub(crate) fn build(
 		self,
 		tree: &Weak<KinematicDataTree>,
 	) -> Result<Transmission, BuildTransmissionError> {
 		// Unwrap Ok because called from tree
@@ -234,25 +212,14 @@
 				|iter| iter.collect(),
 			)?,
 			actuators: self.actuators.0,
 		})
 	}
 }
 
-impl<Joints, Actuators> TransmissionBuilder<Joints, Actuators>
-where
-	Joints: TransmissionJointTrait,
-	Actuators: TransmissionActuatorTrait,
-{
-	/// Gets a reference to the name of the current `TransmissionBuilder`.
-	pub(crate) fn name(&self) -> &String {
-		&self.name
-	}
-}
-
 #[derive(Debug, PartialEq)]
 /// Represents a transmission between a `Joint` and a actuator.
 ///
 /// TODO: DOCS
 /// # TODO: DOCS
 ///  - Link `Joint`
 ///  - Link ROS WIKI
```

### Comparing `robot_description_builder-0.0.1/local_dependencies/robot-description-builder/src/transmission/transmission_actuator.rs` & `robot_description_builder-0.0.2/local_dependencies/robot-description-builder/src/transmission/transmission_actuator.rs`

 * *Files identical despite different names*

### Comparing `robot_description_builder-0.0.1/local_dependencies/robot-description-builder/src/transmission/transmission_joint.rs` & `robot_description_builder-0.0.2/local_dependencies/robot-description-builder/src/transmission/transmission_joint.rs`

 * *Files 1% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 #[derive(Debug, PartialEq, Clone, Default)]
 pub struct TransmissionJointBuilder {
 	joint_name: String,
 	hardware_interfaces: Vec<TransmissionHardwareInterface>,
 }
 
 impl TransmissionJointBuilder {
-	/// TODO: MAKE PUBLIC ?????
+	/// TODO: DOC
 	///
 	/// The minum hardware interfaces is 1 so I require one at creation
 	pub fn new(
 		joint_name: impl Into<String>,
 		hardware_interface: TransmissionHardwareInterface,
 	) -> Self {
 		Self {
```

### Comparing `robot_description_builder-0.0.1/local_dependencies/robot-description-builder/src/transmission/transmission_type.rs` & `robot_description_builder-0.0.2/local_dependencies/robot-description-builder/src/transmission/transmission_type.rs`

 * *Files identical despite different names*

### Comparing `robot_description_builder-0.0.1/.gitignore` & `robot_description_builder-0.0.2/.gitignore`

 * *Files identical despite different names*

### Comparing `robot_description_builder-0.0.1/LICENSE` & `robot_description_builder-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `robot_description_builder-0.0.1/rdf_builder_py.pyi.old` & `robot_description_builder-0.0.2/rdf_builder_py.pyi.old`

 * *Files identical despite different names*

### Comparing `robot_description_builder-0.0.1/src/link/geometry/box_geometry.rs` & `robot_description_builder-0.0.2/src/link/geometry/box_geometry.rs`

 * *Files 15% similar despite different names*

```diff
@@ -1,13 +1,14 @@
-use pyo3::{intern, prelude::*};
+use pyo3::{basic::CompareOp, intern, prelude::*};
 
 use robot_description_builder::link_data::geometry::{BoxGeometry, GeometryInterface};
 
 use super::PyGeometryBase;
 
+#[derive(Debug, Clone)]
 #[pyclass(name = "BoxGeometry", extends = PyGeometryBase, module="robot_description_builder.link.geometry")]
 pub struct PyBoxGeometry {
 	inner: BoxGeometry,
 }
 
 impl PyBoxGeometry {
 	fn new(side0: f32, side1: f32, side2: f32) -> (PyBoxGeometry, PyGeometryBase) {
@@ -22,37 +23,36 @@
 	/// TODO: Names of arguments might be incorrect/Require explanation
 	#[new]
 	#[pyo3(signature = (width, length, height))]
 	fn py_new(width: f32, length: f32, height: f32) -> (PyBoxGeometry, PyGeometryBase) {
 		Self::new(width, length, height)
 	}
 
-	fn __repr__(slf: &PyCell<Self>) -> PyResult<String> {
-		// let module_name = slf
-		// 	.get_type()
-		// 	.getattr(intern!(slf.py(), "__module__"))?
-		// 	.extract::<&str>()?;
-		let class_name = slf
-			.get_type()
-			.getattr(intern!(slf.py(), "__qualname__"))?
+	pub fn __repr__(&self, py: Python<'_>) -> PyResult<String> {
+		let class_name = py
+			.get_type::<Self>()
+			.getattr(intern!(py, "__qualname__"))?
 			.extract::<&str>()?;
 
-		let box_ref = slf.try_borrow()?;
-
 		Ok(format!(
-			// "{}.{}({}, {}, {})",
 			"{}({}, {}, {})",
-			// module_name,
-			class_name,
-			box_ref.inner.side1,
-			box_ref.inner.side2,
-			box_ref.inner.side3
+			class_name, self.inner.side1, self.inner.side2, self.inner.side3
 		))
 	}
 
+	// Might be excessive due to also being implemented on super class
+	fn __richcmp__(&self, other: &Self, op: CompareOp, py: Python<'_>) -> PyObject {
+		match op {
+			CompareOp::Eq => (self.inner == other.inner).into_py(py),
+			CompareOp::Ne => (self.inner != other.inner).into_py(py),
+			// TODO: Consider implementing Gt and Lt based on volume?
+			_ => py.NotImplemented(),
+		}
+	}
+
 	#[getter]
 	fn get_size(&self) -> (f32, f32, f32) {
 		(self.inner.side1, self.inner.side2, self.inner.side3)
 	}
 
 	#[setter]
 	fn set_size(mut slf: PyRefMut<'_, Self>, size: (f32, f32, f32)) {
@@ -62,7 +62,13 @@
 
 		let data = slf.inner.boxed_clone();
 
 		let mut super_class = slf.into_super();
 		super_class.inner = data;
 	}
 }
+
+impl From<BoxGeometry> for PyBoxGeometry {
+	fn from(value: BoxGeometry) -> Self {
+		Self { inner: value }
+	}
+}
```

### Comparing `robot_description_builder-0.0.1/src/link/geometry/cylinder_geometry.rs` & `robot_description_builder-0.0.2/src/link/geometry/cylinder_geometry.rs`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,14 @@
-use pyo3::{intern, prelude::*};
+use pyo3::{basic::CompareOp, intern, prelude::*};
 
 use robot_description_builder::link_data::geometry::{CylinderGeometry, GeometryInterface};
 
 use super::PyGeometryBase;
 
-#[derive(Debug)]
+#[derive(Debug, Clone)]
 #[pyclass(name = "CylinderGeometry", extends = PyGeometryBase, module="robot_description_builder.link.geometry")]
 pub struct PyCylinderGeometry {
 	inner: CylinderGeometry,
 }
 
 impl PyCylinderGeometry {
 	fn new(radius: f32, length: f32) -> (PyCylinderGeometry, PyGeometryBase) {
@@ -22,34 +22,36 @@
 impl PyCylinderGeometry {
 	#[new]
 	#[pyo3(signature = (radius, length))]
 	fn py_new(radius: f32, length: f32) -> (PyCylinderGeometry, PyGeometryBase) {
 		Self::new(radius, length)
 	}
 
-	fn __repr__(slf: &PyCell<Self>) -> PyResult<String> {
-		// let module_name = slf
-		// 	.get_type()
-		// 	.getattr(intern!(slf.py(), "__module__"))?
-		// 	.extract::<&str>()?;
-		let class_name = slf
-			.get_type()
-			.getattr(intern!(slf.py(), "__qualname__"))?
+	pub fn __repr__(&self, py: Python<'_>) -> PyResult<String> {
+		let class_name = py
+			.get_type::<Self>()
+			.getattr(intern!(py, "__qualname__"))?
 			.extract::<&str>()?;
 
-		let cylinder = slf.try_borrow()?;
-
 		Ok(format!(
-			// "{}.{}({}, {})",
 			"{}({}, {})",
-			// module_name,
-			 class_name, cylinder.inner.radius, cylinder.inner.length
+			class_name, self.inner.radius, self.inner.length
 		))
 	}
 
+	// Might be excessive due to also being implemented on super class
+	fn __richcmp__(&self, other: &Self, op: CompareOp, py: Python<'_>) -> PyObject {
+		match op {
+			CompareOp::Eq => (self.inner == other.inner).into_py(py),
+			CompareOp::Ne => (self.inner != other.inner).into_py(py),
+			// TODO: Consider implementing Gt and Lt based on volume?
+			_ => py.NotImplemented(),
+		}
+	}
+
 	/// TODO: Maybe change to dict? or remove
 	#[getter]
 	fn get_size(&self) -> (f32, f32) {
 		(self.inner.radius, self.inner.length)
 	}
 
 	#[getter]
@@ -90,7 +92,13 @@
 
 	//     let data = self_.inner.boxed_clone();
 
 	//     let mut super_class = self_.into_super();
 	//     super_class.inner = data;
 	// }
 }
+
+impl From<CylinderGeometry> for PyCylinderGeometry {
+	fn from(value: CylinderGeometry) -> Self {
+		Self { inner: value }
+	}
+}
```

### Comparing `robot_description_builder-0.0.1/src/link/inertial.rs` & `robot_description_builder-0.0.2/src/link/inertial.rs`

 * *Files 22% similar despite different names*

```diff
@@ -8,15 +8,14 @@
 
 	module.add_class::<PyInertial>()?;
 
 	// parent_module.add_submodule(module)?;
 	Ok(())
 }
 
-/// TODO: Maybe easier to make a python version?
 #[derive(Debug, PartialEq, Clone, Default)]
 #[pyclass(
 	name = "Inertial",
 	module = "robot_description_builder.link",
 	frozen,
 	get_all
 )] // Is set_all ok, since we would need to send the data back to the tree which is weird, immutability is also an option, set_all)]
@@ -53,45 +52,27 @@
 			ixz,
 			iyy,
 			iyz,
 			izz,
 		}
 	}
 
-	/// TODO: Figure this out propperly
-	pub fn __repr__(slf: &PyCell<Self>) -> PyResult<String> {
-		// let module_name = slf
-		// 	.get_type()
-		// 	.getattr(intern!(slf.py(), "__module__"))?
-		// 	.extract::<&str>()?;
-		let class_name = slf
-			.get_type()
-			.getattr(intern!(slf.py(), "__qualname__"))?
+	pub fn __repr__(&self, py: Python<'_>) -> PyResult<String> {
+		let class_name = py
+			.get_type::<Self>()
+			.getattr(intern!(py, "__qualname__"))?
 			.extract::<&str>()?;
 
-		let binding = slf.borrow();
-
 		let mut repr = format!(
-			// "{}.{}(mass = {}, ixx = {}, ixy = {}, ixz = {}, iyy = {}, iyz = {}, izz = {}",
 			"{}(mass = {}, ixx = {}, ixy = {}, ixz = {}, iyy = {}, iyz = {}, izz = {}",
-			// module_name,
-			class_name,
-			binding.mass,
-			binding.ixx,
-			binding.ixy,
-			binding.ixz,
-			binding.iyy,
-			binding.iyz,
-			binding.izz
+			class_name, self.mass, self.ixx, self.ixy, self.ixz, self.iyy, self.iyz, self.izz
 		);
 
-		if let Some(transform) = binding.origin {
-			repr.push_str(
-				", Whoops Something is confusion about repr", // format!(", origin = {}", transform.).as_str()
-			);
+		if let Some(transform) = self.origin {
+			repr.push_str(format!(", origin = {}", transform.__repr__(py)?).as_str());
 		}
 
 		repr.push(')');
 
 		Ok(repr)
 	}
```

### Comparing `robot_description_builder-0.0.1/Cargo.lock` & `robot_description_builder-0.0.2/Cargo.lock`

 * *Files 5% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 # This file is automatically @generated by Cargo.
 # It is not intended for manual editing.
 version = 3
 
 [[package]]
 name = "aho-corasick"
-version = "1.0.1"
+version = "1.0.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "67fc08ce920c31afb70f013dcce1bfc3a3195de6a228474e45e1f145b36f8d04"
+checksum = "43f6cb1bf222025340178f382c426f13757b2960e89779dfcb319c32542a5a41"
 dependencies = [
  "memchr",
 ]
 
 [[package]]
 name = "approx"
 version = "0.5.1"
@@ -73,15 +73,15 @@
 name = "errno"
 version = "0.3.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "4bcfec3a70f97c962c307b2d2c56e358cf1d00b558d74262b5f929ee8cc7e73a"
 dependencies = [
  "errno-dragonfly",
  "libc",
- "windows-sys 0.48.0",
+ "windows-sys",
 ]
 
 [[package]]
 name = "errno-dragonfly"
 version = "0.1.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "aa68f1b12764fab894d2755d2518754e71b4fd80ecfb822714a1206c2aab39bf"
@@ -106,96 +106,93 @@
 name = "indoc"
 version = "1.0.9"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "bfa799dd5ed20a7e349f3b4639aa80d74549c81716d9ec4f994c9b5815598306"
 
 [[package]]
 name = "io-lifetimes"
-version = "1.0.10"
+version = "1.0.11"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "9c66c74d2ae7e79a5a8f7ac924adbe38ee42a859c6539ad869eb51f0b52dc220"
+checksum = "eae7b9aee968036d54dce06cebaefd919e4472e753296daccd6d344e3e2df0c2"
 dependencies = [
  "hermit-abi",
  "libc",
- "windows-sys 0.48.0",
+ "windows-sys",
 ]
 
 [[package]]
 name = "is-terminal"
 version = "0.4.7"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "adcf93614601c8129ddf72e2d5633df827ba6551541c6d8c59520a371475be1f"
 dependencies = [
  "hermit-abi",
  "io-lifetimes",
  "rustix",
- "windows-sys 0.48.0",
+ "windows-sys",
 ]
 
 [[package]]
 name = "itertools"
 version = "0.10.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "b0fd2260e829bddf4cb6ea802289de2f86d6a7a690192fbe91b3f46e0f2c8473"
 dependencies = [
  "either",
 ]
 
 [[package]]
 name = "libc"
-version = "0.2.142"
+version = "0.2.146"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "6a987beff54b60ffa6d51982e1aa1146bc42f19bd26be28b0586f252fccf5317"
+checksum = "f92be4933c13fd498862a9e02a3055f8a8d9c039ce33db97306fd5a6caa7f29b"
 
 [[package]]
 name = "linux-raw-sys"
-version = "0.3.6"
+version = "0.3.8"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "b64f40e5e03e0d54f03845c8197d0291253cdbedfb1cb46b13c2c117554a9f4c"
+checksum = "ef53942eb7bf7ff43a617b3e2c1c4a5ecf5944a7c1bc12d7ee39bbb15e5c1519"
 
 [[package]]
 name = "lock_api"
-version = "0.4.9"
+version = "0.4.10"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "435011366fe56583b16cf956f9df0095b405b82d76425bc8981c0e22e60ec4df"
+checksum = "c1cc9717a20b1bb222f333e6a92fd32f7d8a18ddc5a3191a11af45dcbf4dcd16"
 dependencies = [
  "autocfg",
  "scopeguard",
 ]
 
 [[package]]
 name = "log"
-version = "0.4.17"
+version = "0.4.19"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "abb12e687cfb44aa40f41fc3978ef76448f9b6038cad6aef4259d3c095a2382e"
-dependencies = [
- "cfg-if",
-]
+checksum = "b06a4cde4c0f271a446782e3eff8de789548ce57dbc8eca9292c27f4a42004b4"
 
 [[package]]
 name = "matrixmultiply"
-version = "0.3.5"
+version = "0.3.7"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "f0f0cb8fdceebf83cff284ae2c862792f989731d5eda7bd5b3fd3722003fe8be"
+checksum = "090126dc04f95dc0d1c1c91f61bdd474b3930ca064c1edc8a849da2c6cbe1e77"
 dependencies = [
  "autocfg",
  "rawpointer",
 ]
 
 [[package]]
 name = "memchr"
 version = "2.5.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "2dffe52ecf27772e601905b7522cb4ef790d2cc203488bbd0e2fe85fcb74566d"
 
 [[package]]
 name = "memoffset"
-version = "0.8.0"
+version = "0.9.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "d61c719bcfbcf5d62b3a09efa6088de8c54bc0bfcd3ea7ae39fcc186108b8de1"
+checksum = "5a634b1c61a95585bd15607c6ab0c4e5b226e695ff2800ba0cdccddf208c406c"
 dependencies = [
  "autocfg",
 ]
 
 [[package]]
 name = "nalgebra"
 version = "0.32.2"
@@ -260,110 +257,110 @@
 checksum = "578ede34cf02f8924ab9447f50c28075b4d3e5b269972345e7e0372b38c6cdcd"
 dependencies = [
  "autocfg",
 ]
 
 [[package]]
 name = "once_cell"
-version = "1.17.1"
+version = "1.18.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "b7e5500299e16ebb147ae15a00a942af264cf3688f47923b8fc2cd5858f23ad3"
+checksum = "dd8b5dd2ae5ed71462c540258bedcb51965123ad7e7ccf4b9a8cafaa4a63576d"
 
 [[package]]
 name = "parking_lot"
 version = "0.12.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "3742b2c103b9f06bc9fff0a37ff4912935851bee6d36f3c02bcc755bcfec228f"
 dependencies = [
  "lock_api",
  "parking_lot_core",
 ]
 
 [[package]]
 name = "parking_lot_core"
-version = "0.9.7"
+version = "0.9.8"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "9069cbb9f99e3a5083476ccb29ceb1de18b9118cafa53e90c9551235de2b9521"
+checksum = "93f00c865fe7cabf650081affecd3871070f26767e7b2070a3ffae14c654b447"
 dependencies = [
  "cfg-if",
  "libc",
  "redox_syscall",
  "smallvec",
- "windows-sys 0.45.0",
+ "windows-targets",
 ]
 
 [[package]]
 name = "paste"
 version = "1.0.12"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "9f746c4065a8fa3fe23974dd82f15431cc8d40779821001404d10d2e79ca7d79"
 
 [[package]]
 name = "proc-macro2"
-version = "1.0.56"
+version = "1.0.60"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "2b63bdb0cd06f1f4dedf69b254734f9b45af66e4a031e42a7480257d9898b435"
+checksum = "dec2b086b7a862cf4de201096214fa870344cf922b2b30c167badb3af3195406"
 dependencies = [
  "unicode-ident",
 ]
 
 [[package]]
 name = "pyo3"
-version = "0.18.3"
+version = "0.19.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e3b1ac5b3731ba34fdaa9785f8d74d17448cd18f30cf19e0c7e7b1fdb5272109"
+checksum = "cffef52f74ec3b1a1baf295d9b8fcc3070327aefc39a6d00656b13c1d0b8885c"
 dependencies = [
  "cfg-if",
  "indoc",
  "libc",
  "memoffset",
  "parking_lot",
  "pyo3-build-config",
  "pyo3-ffi",
  "pyo3-macros",
  "unindent",
 ]
 
 [[package]]
 name = "pyo3-build-config"
-version = "0.18.3"
+version = "0.19.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "9cb946f5ac61bb61a5014924910d936ebd2b23b705f7a4a3c40b05c720b079a3"
+checksum = "713eccf888fb05f1a96eb78c0dbc51907fee42b3377272dc902eb38985f418d5"
 dependencies = [
  "once_cell",
  "target-lexicon",
 ]
 
 [[package]]
 name = "pyo3-ffi"
-version = "0.18.3"
+version = "0.19.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "fd4d7c5337821916ea2a1d21d1092e8443cf34879e53a0ac653fbb98f44ff65c"
+checksum = "5b2ecbdcfb01cbbf56e179ce969a048fd7305a66d4cdf3303e0da09d69afe4c3"
 dependencies = [
  "libc",
  "pyo3-build-config",
 ]
 
 [[package]]
 name = "pyo3-macros"
-version = "0.18.3"
+version = "0.19.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "a9d39c55dab3fc5a4b25bbd1ac10a2da452c4aca13bb450f22818a002e29648d"
+checksum = "b78fdc0899f2ea781c463679b20cb08af9247febc8d052de941951024cd8aea0"
 dependencies = [
  "proc-macro2",
  "pyo3-macros-backend",
  "quote",
  "syn 1.0.109",
 ]
 
 [[package]]
 name = "pyo3-macros-backend"
-version = "0.18.3"
+version = "0.19.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "97daff08a4c48320587b5224cc98d609e3c27b6d437315bd40b605c98eeb5918"
+checksum = "60da7b84f1227c3e2fe7593505de274dcf4c8928b4e0a1c23d551a14e4e80a0f"
 dependencies = [
  "proc-macro2",
  "quote",
  "syn 1.0.109",
 ]
 
 [[package]]
@@ -373,94 +370,106 @@
 checksum = "0ce5e73202a820a31f8a0ee32ada5e21029c81fd9e3ebf668a40832e4219d9d1"
 dependencies = [
  "memchr",
 ]
 
 [[package]]
 name = "quote"
-version = "1.0.26"
+version = "1.0.28"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "4424af4bf778aae2051a77b60283332f386554255d722233d09fbfc7e30da2fc"
+checksum = "1b9ab9c7eadfd8df19006f1cf1a4aed13540ed5cbc047010ece5826e10825488"
 dependencies = [
  "proc-macro2",
 ]
 
 [[package]]
 name = "rawpointer"
 version = "0.2.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "60a357793950651c4ed0f3f52338f53b2f809f32d83a07f72909fa13e4c6c1e3"
 
 [[package]]
+name = "rdb-py-macro"
+version = "0.1.0"
+dependencies = [
+ "itertools",
+ "proc-macro2",
+ "quote",
+ "syn 2.0.18",
+]
+
+[[package]]
 name = "redox_syscall"
-version = "0.2.16"
+version = "0.3.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "fb5a58c1855b4b6819d59012155603f0b22ad30cad752600aadfcb695265519a"
+checksum = "567664f262709473930a4bf9e51bf2ebf3348f2e748ccc50dea20646858f8f29"
 dependencies = [
  "bitflags",
 ]
 
 [[package]]
 name = "regex"
-version = "1.8.1"
+version = "1.8.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "af83e617f331cc6ae2da5443c602dfa5af81e517212d9d611a5b3ba1777b5370"
+checksum = "d0ab3ca65655bb1e41f2a8c8cd662eb4fb035e67c3f78da1d61dffe89d07300f"
 dependencies = [
  "aho-corasick",
  "memchr",
  "regex-syntax",
 ]
 
 [[package]]
 name = "regex-syntax"
-version = "0.7.1"
+version = "0.7.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "a5996294f19bd3aae0453a862ad728f60e6600695733dd5df01da90c54363a3c"
+checksum = "436b050e76ed2903236f032a59761c1eb99e1b0aead2c257922771dab1fc8c78"
 
 [[package]]
 name = "robot-description-builder"
-version = "0.0.1"
+version = "0.0.2"
 dependencies = [
  "env_logger",
  "itertools",
  "log",
  "nalgebra",
  "quick-xml",
  "test-log",
  "thiserror",
 ]
 
 [[package]]
 name = "robot-description-builder-py"
-version = "0.0.1"
+version = "0.0.2"
 dependencies = [
  "itertools",
  "pyo3",
+ "rdb-py-macro",
  "robot-description-builder",
+ "thiserror",
 ]
 
 [[package]]
 name = "rustix"
-version = "0.37.18"
+version = "0.37.20"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "8bbfc1d1c7c40c01715f47d71444744a81669ca84e8b63e25a55e169b1f86433"
+checksum = "b96e891d04aa506a6d1f318d2771bcb1c7dfda84e126660ace067c9b474bb2c0"
 dependencies = [
  "bitflags",
  "errno",
  "io-lifetimes",
  "libc",
  "linux-raw-sys",
- "windows-sys 0.48.0",
+ "windows-sys",
 ]
 
 [[package]]
 name = "safe_arch"
-version = "0.6.0"
+version = "0.7.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "794821e4ccb0d9f979512f9c1973480123f9bd62a90d74ab0f9426fcf8f4a529"
+checksum = "62a7484307bd40f8f7ccbacccac730108f2cae119a3b11c74485b48aa9ea650f"
 dependencies = [
  "bytemuck",
 ]
 
 [[package]]
 name = "scopeguard"
 version = "1.1.0"
@@ -495,17 +504,17 @@
  "proc-macro2",
  "quote",
  "unicode-ident",
 ]
 
 [[package]]
 name = "syn"
-version = "2.0.15"
+version = "2.0.18"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "a34fcf3e8b60f57e6a14301a2e916d323af98b0ea63c599441eec8558660c822"
+checksum = "32d41677bcbe24c20c52e7c70b0d8db04134c5d1066bf98662e2871ad200ea3e"
 dependencies = [
  "proc-macro2",
  "quote",
  "unicode-ident",
 ]
 
 [[package]]
@@ -521,17 +530,17 @@
 checksum = "be55cf8942feac5c765c2c993422806843c9a9a45d4d5c407ad6dd2ea95eb9b6"
 dependencies = [
  "winapi-util",
 ]
 
 [[package]]
 name = "test-log"
-version = "0.2.11"
+version = "0.2.12"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "38f0c854faeb68a048f0f2dc410c5ddae3bf83854ef0e4977d58306a5edef50e"
+checksum = "d9601d162c1d77e62c1ea0bc8116cd1caf143ce3af947536c3c9052a1677fe0c"
 dependencies = [
  "proc-macro2",
  "quote",
  "syn 1.0.109",
 ]
 
 [[package]]
@@ -547,40 +556,40 @@
 name = "thiserror-impl"
 version = "1.0.40"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "f9456a42c5b0d803c8cd86e73dd7cc9edd429499f37a3550d286d5e86720569f"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.15",
+ "syn 2.0.18",
 ]
 
 [[package]]
 name = "typenum"
 version = "1.16.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "497961ef93d974e23eb6f433eb5fe1b7930b659f06d12dec6fc44a8f554c0bba"
 
 [[package]]
 name = "unicode-ident"
-version = "1.0.8"
+version = "1.0.9"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e5464a87b239f13a63a501f2701565754bae92d243d4bb7eb12f6d57d2269bf4"
+checksum = "b15811caf2415fb889178633e7724bad2509101cde276048e013b9def5e51fa0"
 
 [[package]]
 name = "unindent"
 version = "0.1.11"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e1766d682d402817b5ac4490b3c3002d91dfa0d22812f341609f97b08757359c"
 
 [[package]]
 name = "wide"
-version = "0.7.8"
+version = "0.7.10"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "b689b6c49d6549434bf944e6b0f39238cf63693cb7a147e9d887507fffa3b223"
+checksum = "40018623e2dba2602a9790faba8d33f2ebdebf4b86561b83928db735f8784728"
 dependencies = [
  "bytemuck",
  "safe_arch",
 ]
 
 [[package]]
 name = "winapi"
@@ -611,136 +620,70 @@
 name = "winapi-x86_64-pc-windows-gnu"
 version = "0.4.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "712e227841d057c1ee1cd2fb22fa7e5a5461ae8e48fa2ca79ec42cfc1931183f"
 
 [[package]]
 name = "windows-sys"
-version = "0.45.0"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "75283be5efb2831d37ea142365f009c02ec203cd29a3ebecbc093d52315b66d0"
-dependencies = [
- "windows-targets 0.42.2",
-]
-
-[[package]]
-name = "windows-sys"
 version = "0.48.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "677d2418bec65e3338edb076e806bc1ec15693c5d0104683f2efe857f61056a9"
 dependencies = [
- "windows-targets 0.48.0",
-]
-
-[[package]]
-name = "windows-targets"
-version = "0.42.2"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "8e5180c00cd44c9b1c88adb3693291f1cd93605ded80c250a75d472756b4d071"
-dependencies = [
- "windows_aarch64_gnullvm 0.42.2",
- "windows_aarch64_msvc 0.42.2",
- "windows_i686_gnu 0.42.2",
- "windows_i686_msvc 0.42.2",
- "windows_x86_64_gnu 0.42.2",
- "windows_x86_64_gnullvm 0.42.2",
- "windows_x86_64_msvc 0.42.2",
+ "windows-targets",
 ]
 
 [[package]]
 name = "windows-targets"
 version = "0.48.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "7b1eb6f0cd7c80c79759c929114ef071b87354ce476d9d94271031c0497adfd5"
 dependencies = [
- "windows_aarch64_gnullvm 0.48.0",
- "windows_aarch64_msvc 0.48.0",
- "windows_i686_gnu 0.48.0",
- "windows_i686_msvc 0.48.0",
- "windows_x86_64_gnu 0.48.0",
- "windows_x86_64_gnullvm 0.48.0",
- "windows_x86_64_msvc 0.48.0",
+ "windows_aarch64_gnullvm",
+ "windows_aarch64_msvc",
+ "windows_i686_gnu",
+ "windows_i686_msvc",
+ "windows_x86_64_gnu",
+ "windows_x86_64_gnullvm",
+ "windows_x86_64_msvc",
 ]
 
 [[package]]
 name = "windows_aarch64_gnullvm"
-version = "0.42.2"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "597a5118570b68bc08d8d59125332c54f1ba9d9adeedeef5b99b02ba2b0698f8"
-
-[[package]]
-name = "windows_aarch64_gnullvm"
 version = "0.48.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "91ae572e1b79dba883e0d315474df7305d12f569b400fcf90581b06062f7e1bc"
 
 [[package]]
 name = "windows_aarch64_msvc"
-version = "0.42.2"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e08e8864a60f06ef0d0ff4ba04124db8b0fb3be5776a5cd47641e942e58c4d43"
-
-[[package]]
-name = "windows_aarch64_msvc"
 version = "0.48.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "b2ef27e0d7bdfcfc7b868b317c1d32c641a6fe4629c171b8928c7b08d98d7cf3"
 
 [[package]]
 name = "windows_i686_gnu"
-version = "0.42.2"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "c61d927d8da41da96a81f029489353e68739737d3beca43145c8afec9a31a84f"
-
-[[package]]
-name = "windows_i686_gnu"
 version = "0.48.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "622a1962a7db830d6fd0a69683c80a18fda201879f0f447f065a3b7467daa241"
 
 [[package]]
 name = "windows_i686_msvc"
-version = "0.42.2"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "44d840b6ec649f480a41c8d80f9c65108b92d89345dd94027bfe06ac444d1060"
-
-[[package]]
-name = "windows_i686_msvc"
 version = "0.48.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "4542c6e364ce21bf45d69fdd2a8e455fa38d316158cfd43b3ac1c5b1b19f8e00"
 
 [[package]]
 name = "windows_x86_64_gnu"
-version = "0.42.2"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "8de912b8b8feb55c064867cf047dda097f92d51efad5b491dfb98f6bbb70cb36"
-
-[[package]]
-name = "windows_x86_64_gnu"
 version = "0.48.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "ca2b8a661f7628cbd23440e50b05d705db3686f894fc9580820623656af974b1"
 
 [[package]]
 name = "windows_x86_64_gnullvm"
-version = "0.42.2"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "26d41b46a36d453748aedef1486d5c7a85db22e56aff34643984ea85514e94a3"
-
-[[package]]
-name = "windows_x86_64_gnullvm"
 version = "0.48.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "7896dbc1f41e08872e9d5e8f8baa8fdd2677f29468c4e156210174edc7f7b953"
 
 [[package]]
 name = "windows_x86_64_msvc"
-version = "0.42.2"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "9aec5da331524158c6d1a4ac0ab1541149c0b9505fde06423b02f5ef0106b9f0"
-
-[[package]]
-name = "windows_x86_64_msvc"
 version = "0.48.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "1a515f5799fe4961cb532f983ce2b23082366b898e52ffbce459c86f67c8378a"
```

