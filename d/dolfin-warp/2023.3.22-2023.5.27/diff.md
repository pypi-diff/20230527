# Comparing `tmp/dolfin_warp-2023.3.22.tar.gz` & `tmp/dolfin_warp-2023.5.27.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dolfin_warp-2023.3.22.tar", last modified: Wed Mar 22 11:45:47 2023, max compression
+gzip compressed data, was "dolfin_warp-2023.5.27.tar", last modified: Sat May 27 21:27:19 2023, max compression
```

## Comparing `dolfin_warp-2023.3.22.tar` & `dolfin_warp-2023.5.27.tar`

### file list

```diff
@@ -1,73 +1,73 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-22 11:45:47.548928 dolfin_warp-2023.3.22/
--rw-rw-rw-   0 root         (0) root         (0)     7651 2023-03-22 11:45:35.000000 dolfin_warp-2023.3.22/LICENSE
--rw-r--r--   0 root         (0) root         (0)     1175 2023-03-22 11:45:47.547928 dolfin_warp-2023.3.22/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      468 2023-03-22 11:45:35.000000 dolfin_warp-2023.3.22/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-22 11:45:47.545928 dolfin_warp-2023.3.22/dolfin_warp/
--rw-rw-rw-   0 root         (0) root         (0)     1040 2023-03-22 11:45:35.000000 dolfin_warp-2023.3.22/dolfin_warp/Energy.py
--rw-rw-rw-   0 root         (0) root         (0)     3617 2023-03-22 11:45:35.000000 dolfin_warp-2023.3.22/dolfin_warp/Energy_Continuous.py
--rw-rw-rw-   0 root         (0) root         (0)    12839 2023-03-22 11:45:35.000000 dolfin_warp-2023.3.22/dolfin_warp/Energy_Continuous_GeneratedImage.py
--rw-rw-rw-   0 root         (0) root         (0)     6306 2023-03-22 11:45:35.000000 dolfin_warp-2023.3.22/dolfin_warp/Energy_Continuous_Regularization.py
--rw-rw-rw-   0 root         (0) root         (0)    15101 2023-03-22 11:45:35.000000 dolfin_warp-2023.3.22/dolfin_warp/Energy_Continuous_WarpedImage.py
--rw-rw-rw-   0 root         (0) root         (0)      733 2023-03-22 11:45:35.000000 dolfin_warp-2023.3.22/dolfin_warp/Energy_Discrete.py
--rw-rw-rw-   0 root         (0) root         (0)     5306 2023-03-22 11:45:35.000000 dolfin_warp-2023.3.22/dolfin_warp/Energy_Discrete_SimpleRegularization.py
--rw-rw-rw-   0 root         (0) root         (0)    18931 2023-03-22 11:45:35.000000 dolfin_warp-2023.3.22/dolfin_warp/Energy_Discrete_SurfaceRegularization.py
--rw-rw-rw-   0 root         (0) root         (0)     9502 2023-03-22 11:45:35.000000 dolfin_warp-2023.3.22/dolfin_warp/Energy_Discrete_VolumeRegularization.py
--rw-rw-rw-   0 root         (0) root         (0)      696 2023-03-22 11:45:35.000000 dolfin_warp-2023.3.22/dolfin_warp/FilesSeries.py
--rw-rw-rw-   0 root         (0) root         (0)     3965 2023-03-22 11:45:35.000000 dolfin_warp-2023.3.22/dolfin_warp/FilesSeries_Images.py
--rw-rw-rw-   0 root         (0) root         (0)     3140 2023-03-22 11:45:35.000000 dolfin_warp-2023.3.22/dolfin_warp/FilesSeries_Meshes.py
--rw-rw-rw-   0 root         (0) root         (0)    12924 2023-03-22 11:45:35.000000 dolfin_warp-2023.3.22/dolfin_warp/ImageIterator.py
--rw-rw-rw-   0 root         (0) root         (0)     5430 2023-03-22 11:45:35.000000 dolfin_warp-2023.3.22/dolfin_warp/ModalAnalysis.py
--rw-rw-rw-   0 root         (0) root         (0)     3932 2023-03-22 11:45:35.000000 dolfin_warp-2023.3.22/dolfin_warp/MotionModel.py
--rw-rw-rw-   0 root         (0) root         (0)      770 2023-03-22 11:45:35.000000 dolfin_warp-2023.3.22/dolfin_warp/NonlinearSolver.py
--rw-rw-rw-   0 root         (0) root         (0)    14134 2023-03-22 11:45:35.000000 dolfin_warp-2023.3.22/dolfin_warp/NonlinearSolver_CMA.py
--rw-rw-rw-   0 root         (0) root         (0)    10064 2023-03-22 11:45:35.000000 dolfin_warp-2023.3.22/dolfin_warp/NonlinearSolver_Newton.py
--rw-rw-rw-   0 root         (0) root         (0)    11265 2023-03-22 11:45:35.000000 dolfin_warp-2023.3.22/dolfin_warp/NonlinearSolver_ReducedKinematicsNewton.py
--rw-rw-rw-   0 root         (0) root         (0)     8777 2023-03-22 11:45:35.000000 dolfin_warp-2023.3.22/dolfin_warp/NonlinearSolver_Relaxation.py
--rw-rw-rw-   0 root         (0) root         (0)      696 2023-03-22 11:45:35.000000 dolfin_warp-2023.3.22/dolfin_warp/Problem.py
--rw-rw-rw-   0 root         (0) root         (0)     8339 2023-03-22 11:45:35.000000 dolfin_warp-2023.3.22/dolfin_warp/Problem_Warping.py
--rw-rw-rw-   0 root         (0) root         (0)     2324 2023-03-22 11:45:35.000000 dolfin_warp-2023.3.22/dolfin_warp/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)     3259 2023-03-22 11:45:35.000000 dolfin_warp-2023.3.22/dolfin_warp/compute_best_regularization_strength.py
--rw-rw-rw-   0 root         (0) root         (0)     8393 2023-03-22 11:45:35.000000 dolfin_warp-2023.3.22/dolfin_warp/compute_displacement_error.py
--rwxrwxrwx   0 root         (0) root         (0)     2308 2023-03-22 11:45:35.000000 dolfin_warp-2023.3.22/dolfin_warp/compute_displacement_error_field.py
--rwxrwxrwx   0 root         (0) root         (0)     1822 2023-03-22 11:45:35.000000 dolfin_warp-2023.3.22/dolfin_warp/compute_displacement_infinity_norm.py
--rw-rw-rw-   0 root         (0) root         (0)     2267 2023-03-22 11:45:35.000000 dolfin_warp-2023.3.22/dolfin_warp/compute_displacements_from_ref.py
--rw-rw-rw-   0 root         (0) root         (0)     9058 2023-03-22 11:45:35.000000 dolfin_warp-2023.3.22/dolfin_warp/compute_downsampled_images.py
--rw-rw-rw-   0 root         (0) root         (0)     1852 2023-03-22 11:45:35.000000 dolfin_warp-2023.3.22/dolfin_warp/compute_energies_normalization.py
--rw-rw-rw-   0 root         (0) root         (0)     2513 2023-03-22 11:45:35.000000 dolfin_warp-2023.3.22/dolfin_warp/compute_equalized_images.py
--rw-rw-rw-   0 root         (0) root         (0)     3539 2023-03-22 11:45:35.000000 dolfin_warp-2023.3.22/dolfin_warp/compute_normalized_images.py
--rw-rw-rw-   0 root         (0) root         (0)     9535 2023-03-22 11:45:35.000000 dolfin_warp-2023.3.22/dolfin_warp/compute_projected_image.py
--rw-rw-rw-   0 root         (0) root         (0)     5502 2023-03-22 11:45:35.000000 dolfin_warp-2023.3.22/dolfin_warp/compute_quadrature_degree.py
--rw-rw-rw-   0 root         (0) root         (0)    10916 2023-03-22 11:45:35.000000 dolfin_warp-2023.3.22/dolfin_warp/compute_regularization_energies.py
--rw-rw-rw-   0 root         (0) root         (0)     7718 2023-03-22 11:45:35.000000 dolfin_warp-2023.3.22/dolfin_warp/compute_selective_image_gradient.py
--rwxrwxrwx   0 root         (0) root         (0)     6268 2023-03-22 11:45:35.000000 dolfin_warp-2023.3.22/dolfin_warp/compute_strain_error.py
--rw-rw-rw-   0 root         (0) root         (0)    20854 2023-03-22 11:45:35.000000 dolfin_warp-2023.3.22/dolfin_warp/compute_strains.py
--rw-rw-rw-   0 root         (0) root         (0)     3098 2023-03-22 11:45:35.000000 dolfin_warp-2023.3.22/dolfin_warp/compute_unwarped_images.py
--rw-rw-rw-   0 root         (0) root         (0)     4962 2023-03-22 11:45:35.000000 dolfin_warp-2023.3.22/dolfin_warp/compute_warped_images.py
--rw-rw-rw-   0 root         (0) root         (0)     3892 2023-03-22 11:45:35.000000 dolfin_warp-2023.3.22/dolfin_warp/compute_warped_mesh.py
--rw-rw-rw-   0 root         (0) root         (0)    10203 2023-03-22 11:45:35.000000 dolfin_warp-2023.3.22/dolfin_warp/expressions_char_func_cpp.py
--rw-rw-rw-   0 root         (0) root         (0)    32381 2023-03-22 11:45:35.000000 dolfin_warp-2023.3.22/dolfin_warp/expressions_generated_images_cpp.py
--rw-rw-rw-   0 root         (0) root         (0)    15850 2023-03-22 11:45:35.000000 dolfin_warp-2023.3.22/dolfin_warp/expressions_images_cpp.py
--rw-rw-rw-   0 root         (0) root         (0)    13739 2023-03-22 11:45:35.000000 dolfin_warp-2023.3.22/dolfin_warp/expressions_images_py.py
--rw-rw-rw-   0 root         (0) root         (0)     1407 2023-03-22 11:45:35.000000 dolfin_warp-2023.3.22/dolfin_warp/expressions_static_scaling_cpp.py
--rw-rw-rw-   0 root         (0) root         (0)     7369 2023-03-22 11:45:35.000000 dolfin_warp-2023.3.22/dolfin_warp/generate_images.py
--rw-rw-rw-   0 root         (0) root         (0)    22180 2023-03-22 11:45:35.000000 dolfin_warp-2023.3.22/dolfin_warp/generate_images_Image.py
--rw-rw-rw-   0 root         (0) root         (0)    12130 2023-03-22 11:45:35.000000 dolfin_warp-2023.3.22/dolfin_warp/generate_images_Mapping.py
--rw-rw-rw-   0 root         (0) root         (0)     1462 2023-03-22 11:45:35.000000 dolfin_warp-2023.3.22/dolfin_warp/generate_images_Noise.py
--rw-rw-rw-   0 root         (0) root         (0)     6603 2023-03-22 11:45:35.000000 dolfin_warp-2023.3.22/dolfin_warp/generate_undersampled_images.py
--rw-rw-rw-   0 root         (0) root         (0)     2034 2023-03-22 11:45:35.000000 dolfin_warp-2023.3.22/dolfin_warp/get_centroids.py
--rw-rw-rw-   0 root         (0) root         (0)     4769 2023-03-22 11:45:35.000000 dolfin_warp-2023.3.22/dolfin_warp/plot_binned_strains_vs_radius.py
--rw-rw-rw-   0 root         (0) root         (0)     2218 2023-03-22 11:45:35.000000 dolfin_warp-2023.3.22/dolfin_warp/plot_displacement_error.py
--rw-rw-rw-   0 root         (0) root         (0)     6896 2023-03-22 11:45:35.000000 dolfin_warp-2023.3.22/dolfin_warp/plot_regional_strains.py
--rw-rw-rw-   0 root         (0) root         (0)     4806 2023-03-22 11:45:35.000000 dolfin_warp-2023.3.22/dolfin_warp/plot_strains.py
--rw-rw-rw-   0 root         (0) root         (0)     3747 2023-03-22 11:45:35.000000 dolfin_warp-2023.3.22/dolfin_warp/plot_strains_vs_radius.py
--rw-rw-rw-   0 root         (0) root         (0)     2177 2023-03-22 11:45:35.000000 dolfin_warp-2023.3.22/dolfin_warp/plot_twist_vs_height.py
--rw-rw-rw-   0 root         (0) root         (0)    17792 2023-03-22 11:45:35.000000 dolfin_warp-2023.3.22/dolfin_warp/warp.py
--rw-rw-rw-   0 root         (0) root         (0)     6973 2023-03-22 11:45:35.000000 dolfin_warp-2023.3.22/dolfin_warp/warp_and_refine.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-22 11:45:47.547928 dolfin_warp-2023.3.22/dolfin_warp.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1175 2023-03-22 11:45:47.000000 dolfin_warp-2023.3.22/dolfin_warp.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2504 2023-03-22 11:45:47.000000 dolfin_warp-2023.3.22/dolfin_warp.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-03-22 11:45:47.000000 dolfin_warp-2023.3.22/dolfin_warp.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       95 2023-03-22 11:45:47.000000 dolfin_warp-2023.3.22/dolfin_warp.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       12 2023-03-22 11:45:47.000000 dolfin_warp-2023.3.22/dolfin_warp.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-03-22 11:45:47.548928 dolfin_warp-2023.3.22/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)      891 2023-03-22 11:45:35.000000 dolfin_warp-2023.3.22/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-27 21:27:19.234854 dolfin_warp-2023.5.27/
+-rw-rw-rw-   0 root         (0) root         (0)     7651 2023-05-27 21:27:07.000000 dolfin_warp-2023.5.27/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     1519 2023-05-27 21:27:19.233854 dolfin_warp-2023.5.27/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      701 2023-05-27 21:27:07.000000 dolfin_warp-2023.5.27/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-27 21:27:19.231854 dolfin_warp-2023.5.27/dolfin_warp/
+-rw-rw-rw-   0 root         (0) root         (0)     1040 2023-05-27 21:27:07.000000 dolfin_warp-2023.5.27/dolfin_warp/Energy.py
+-rw-rw-rw-   0 root         (0) root         (0)     3617 2023-05-27 21:27:07.000000 dolfin_warp-2023.5.27/dolfin_warp/Energy_Continuous.py
+-rw-rw-rw-   0 root         (0) root         (0)    12839 2023-05-27 21:27:07.000000 dolfin_warp-2023.5.27/dolfin_warp/Energy_Continuous_GeneratedImage.py
+-rw-rw-rw-   0 root         (0) root         (0)     6306 2023-05-27 21:27:07.000000 dolfin_warp-2023.5.27/dolfin_warp/Energy_Continuous_Regularization.py
+-rw-rw-rw-   0 root         (0) root         (0)    15101 2023-05-27 21:27:07.000000 dolfin_warp-2023.5.27/dolfin_warp/Energy_Continuous_WarpedImage.py
+-rw-rw-rw-   0 root         (0) root         (0)      733 2023-05-27 21:27:07.000000 dolfin_warp-2023.5.27/dolfin_warp/Energy_Discrete.py
+-rw-rw-rw-   0 root         (0) root         (0)     5306 2023-05-27 21:27:07.000000 dolfin_warp-2023.5.27/dolfin_warp/Energy_Discrete_SimpleRegularization.py
+-rw-rw-rw-   0 root         (0) root         (0)    18931 2023-05-27 21:27:07.000000 dolfin_warp-2023.5.27/dolfin_warp/Energy_Discrete_SurfaceRegularization.py
+-rw-rw-rw-   0 root         (0) root         (0)     9502 2023-05-27 21:27:07.000000 dolfin_warp-2023.5.27/dolfin_warp/Energy_Discrete_VolumeRegularization.py
+-rw-rw-rw-   0 root         (0) root         (0)      696 2023-05-27 21:27:07.000000 dolfin_warp-2023.5.27/dolfin_warp/FilesSeries.py
+-rw-rw-rw-   0 root         (0) root         (0)     3965 2023-05-27 21:27:07.000000 dolfin_warp-2023.5.27/dolfin_warp/FilesSeries_Images.py
+-rw-rw-rw-   0 root         (0) root         (0)     3140 2023-05-27 21:27:07.000000 dolfin_warp-2023.5.27/dolfin_warp/FilesSeries_Meshes.py
+-rw-rw-rw-   0 root         (0) root         (0)    12924 2023-05-27 21:27:07.000000 dolfin_warp-2023.5.27/dolfin_warp/ImageIterator.py
+-rw-rw-rw-   0 root         (0) root         (0)     5430 2023-05-27 21:27:07.000000 dolfin_warp-2023.5.27/dolfin_warp/ModalAnalysis.py
+-rw-rw-rw-   0 root         (0) root         (0)     3932 2023-05-27 21:27:07.000000 dolfin_warp-2023.5.27/dolfin_warp/MotionModel.py
+-rw-rw-rw-   0 root         (0) root         (0)      770 2023-05-27 21:27:07.000000 dolfin_warp-2023.5.27/dolfin_warp/NonlinearSolver.py
+-rw-rw-rw-   0 root         (0) root         (0)    14134 2023-05-27 21:27:07.000000 dolfin_warp-2023.5.27/dolfin_warp/NonlinearSolver_CMA.py
+-rw-rw-rw-   0 root         (0) root         (0)    10064 2023-05-27 21:27:07.000000 dolfin_warp-2023.5.27/dolfin_warp/NonlinearSolver_Newton.py
+-rw-rw-rw-   0 root         (0) root         (0)    11265 2023-05-27 21:27:07.000000 dolfin_warp-2023.5.27/dolfin_warp/NonlinearSolver_ReducedKinematicsNewton.py
+-rw-rw-rw-   0 root         (0) root         (0)     8782 2023-05-27 21:27:07.000000 dolfin_warp-2023.5.27/dolfin_warp/NonlinearSolver_Relaxation.py
+-rw-rw-rw-   0 root         (0) root         (0)      696 2023-05-27 21:27:07.000000 dolfin_warp-2023.5.27/dolfin_warp/Problem.py
+-rw-rw-rw-   0 root         (0) root         (0)     8339 2023-05-27 21:27:07.000000 dolfin_warp-2023.5.27/dolfin_warp/Problem_Warping.py
+-rw-rw-rw-   0 root         (0) root         (0)     2324 2023-05-27 21:27:07.000000 dolfin_warp-2023.5.27/dolfin_warp/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)     3259 2023-05-27 21:27:07.000000 dolfin_warp-2023.5.27/dolfin_warp/compute_best_regularization_strength.py
+-rw-rw-rw-   0 root         (0) root         (0)    13920 2023-05-27 21:27:07.000000 dolfin_warp-2023.5.27/dolfin_warp/compute_displacement_error.py
+-rwxrwxrwx   0 root         (0) root         (0)     2308 2023-05-27 21:27:07.000000 dolfin_warp-2023.5.27/dolfin_warp/compute_displacement_error_field.py
+-rwxrwxrwx   0 root         (0) root         (0)     1822 2023-05-27 21:27:07.000000 dolfin_warp-2023.5.27/dolfin_warp/compute_displacement_infinity_norm.py
+-rw-rw-rw-   0 root         (0) root         (0)     2267 2023-05-27 21:27:07.000000 dolfin_warp-2023.5.27/dolfin_warp/compute_displacements_from_ref.py
+-rw-rw-rw-   0 root         (0) root         (0)     9058 2023-05-27 21:27:07.000000 dolfin_warp-2023.5.27/dolfin_warp/compute_downsampled_images.py
+-rw-rw-rw-   0 root         (0) root         (0)     1852 2023-05-27 21:27:07.000000 dolfin_warp-2023.5.27/dolfin_warp/compute_energies_normalization.py
+-rw-rw-rw-   0 root         (0) root         (0)     2513 2023-05-27 21:27:07.000000 dolfin_warp-2023.5.27/dolfin_warp/compute_equalized_images.py
+-rw-rw-rw-   0 root         (0) root         (0)     3539 2023-05-27 21:27:07.000000 dolfin_warp-2023.5.27/dolfin_warp/compute_normalized_images.py
+-rw-rw-rw-   0 root         (0) root         (0)     9535 2023-05-27 21:27:07.000000 dolfin_warp-2023.5.27/dolfin_warp/compute_projected_image.py
+-rw-rw-rw-   0 root         (0) root         (0)     5502 2023-05-27 21:27:07.000000 dolfin_warp-2023.5.27/dolfin_warp/compute_quadrature_degree.py
+-rw-rw-rw-   0 root         (0) root         (0)    10916 2023-05-27 21:27:07.000000 dolfin_warp-2023.5.27/dolfin_warp/compute_regularization_energies.py
+-rw-rw-rw-   0 root         (0) root         (0)     7718 2023-05-27 21:27:07.000000 dolfin_warp-2023.5.27/dolfin_warp/compute_selective_image_gradient.py
+-rwxrwxrwx   0 root         (0) root         (0)     6268 2023-05-27 21:27:07.000000 dolfin_warp-2023.5.27/dolfin_warp/compute_strain_error.py
+-rw-rw-rw-   0 root         (0) root         (0)    20854 2023-05-27 21:27:07.000000 dolfin_warp-2023.5.27/dolfin_warp/compute_strains.py
+-rw-rw-rw-   0 root         (0) root         (0)     3098 2023-05-27 21:27:07.000000 dolfin_warp-2023.5.27/dolfin_warp/compute_unwarped_images.py
+-rw-rw-rw-   0 root         (0) root         (0)     4962 2023-05-27 21:27:07.000000 dolfin_warp-2023.5.27/dolfin_warp/compute_warped_images.py
+-rw-rw-rw-   0 root         (0) root         (0)     3892 2023-05-27 21:27:07.000000 dolfin_warp-2023.5.27/dolfin_warp/compute_warped_mesh.py
+-rw-rw-rw-   0 root         (0) root         (0)    10203 2023-05-27 21:27:07.000000 dolfin_warp-2023.5.27/dolfin_warp/expressions_char_func_cpp.py
+-rw-rw-rw-   0 root         (0) root         (0)    32381 2023-05-27 21:27:07.000000 dolfin_warp-2023.5.27/dolfin_warp/expressions_generated_images_cpp.py
+-rw-rw-rw-   0 root         (0) root         (0)    15850 2023-05-27 21:27:07.000000 dolfin_warp-2023.5.27/dolfin_warp/expressions_images_cpp.py
+-rw-rw-rw-   0 root         (0) root         (0)    13739 2023-05-27 21:27:07.000000 dolfin_warp-2023.5.27/dolfin_warp/expressions_images_py.py
+-rw-rw-rw-   0 root         (0) root         (0)     1407 2023-05-27 21:27:07.000000 dolfin_warp-2023.5.27/dolfin_warp/expressions_static_scaling_cpp.py
+-rw-rw-rw-   0 root         (0) root         (0)     7369 2023-05-27 21:27:07.000000 dolfin_warp-2023.5.27/dolfin_warp/generate_images.py
+-rw-rw-rw-   0 root         (0) root         (0)    22180 2023-05-27 21:27:07.000000 dolfin_warp-2023.5.27/dolfin_warp/generate_images_Image.py
+-rw-rw-rw-   0 root         (0) root         (0)    12130 2023-05-27 21:27:07.000000 dolfin_warp-2023.5.27/dolfin_warp/generate_images_Mapping.py
+-rw-rw-rw-   0 root         (0) root         (0)     1462 2023-05-27 21:27:07.000000 dolfin_warp-2023.5.27/dolfin_warp/generate_images_Noise.py
+-rw-rw-rw-   0 root         (0) root         (0)     6603 2023-05-27 21:27:07.000000 dolfin_warp-2023.5.27/dolfin_warp/generate_undersampled_images.py
+-rw-rw-rw-   0 root         (0) root         (0)     2034 2023-05-27 21:27:07.000000 dolfin_warp-2023.5.27/dolfin_warp/get_centroids.py
+-rw-rw-rw-   0 root         (0) root         (0)     4769 2023-05-27 21:27:07.000000 dolfin_warp-2023.5.27/dolfin_warp/plot_binned_strains_vs_radius.py
+-rw-rw-rw-   0 root         (0) root         (0)     2218 2023-05-27 21:27:07.000000 dolfin_warp-2023.5.27/dolfin_warp/plot_displacement_error.py
+-rw-rw-rw-   0 root         (0) root         (0)     6896 2023-05-27 21:27:07.000000 dolfin_warp-2023.5.27/dolfin_warp/plot_regional_strains.py
+-rw-rw-rw-   0 root         (0) root         (0)     4806 2023-05-27 21:27:07.000000 dolfin_warp-2023.5.27/dolfin_warp/plot_strains.py
+-rw-rw-rw-   0 root         (0) root         (0)     3747 2023-05-27 21:27:07.000000 dolfin_warp-2023.5.27/dolfin_warp/plot_strains_vs_radius.py
+-rw-rw-rw-   0 root         (0) root         (0)     2177 2023-05-27 21:27:07.000000 dolfin_warp-2023.5.27/dolfin_warp/plot_twist_vs_height.py
+-rw-rw-rw-   0 root         (0) root         (0)    17792 2023-05-27 21:27:07.000000 dolfin_warp-2023.5.27/dolfin_warp/warp.py
+-rw-rw-rw-   0 root         (0) root         (0)     6973 2023-05-27 21:27:07.000000 dolfin_warp-2023.5.27/dolfin_warp/warp_and_refine.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-27 21:27:19.233854 dolfin_warp-2023.5.27/dolfin_warp.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1519 2023-05-27 21:27:19.000000 dolfin_warp-2023.5.27/dolfin_warp.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2504 2023-05-27 21:27:19.000000 dolfin_warp-2023.5.27/dolfin_warp.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-27 21:27:19.000000 dolfin_warp-2023.5.27/dolfin_warp.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       95 2023-05-27 21:27:19.000000 dolfin_warp-2023.5.27/dolfin_warp.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       12 2023-05-27 21:27:19.000000 dolfin_warp-2023.5.27/dolfin_warp.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-05-27 21:27:19.234854 dolfin_warp-2023.5.27/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      891 2023-05-27 21:27:07.000000 dolfin_warp-2023.5.27/setup.py
```

### Comparing `dolfin_warp-2023.3.22/LICENSE` & `dolfin_warp-2023.5.27/LICENSE`

 * *Files identical despite different names*

### Comparing `dolfin_warp-2023.3.22/PKG-INFO` & `dolfin_warp-2023.5.27/dolfin_warp.egg-info/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,22 +1,24 @@
 Metadata-Version: 2.1
-Name: dolfin_warp
-Version: 2023.3.22
-Summary: A set of FEniCS- and VTK-based python tools for Finite Element Digital Image Correlation, basically implementing the method described in [[Genet et al., 2018, Medical Image Analysis]](https://www.medicalimageanalysisjournal.com/article/S1361-8415(18)30534-6/fulltext).
+Name: dolfin-warp
+Version: 2023.5.27
+Summary: A set of FEniCS- and VTK-based python tools for Finite Element Digital Image Correlation, basically implementing the method described in [[Genet, Stoeck, von Deuster, Lee & Kozerke (2018). Equilibrated Warping: Finite Element Image Registration with Finite Strain Equilibrium Gap Regularization. Medical Image Analysis, 50, 1–22.]](https://doi.org/10.1016/j.media.2018.07.007).
 Home-page: https://gitlab.inria.fr/mgenet/dolfin_warp
 Author: Martin Genet
 Author-email: martin.genet@polytechnique.edu
 License: GPLv3
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # dolfin_warp
-A set of FEniCS- and VTK-based python tools for Finite Element Digital Image Correlation, basically implementing the method described in [[Genet et al., 2018, Medical Image Analysis]](https://www.medicalimageanalysisjournal.com/article/S1361-8415(18)30534-6/fulltext).
+A set of FEniCS- and VTK-based python tools for Finite Element Digital Image Correlation, basically implementing the method described in [[Genet, Stoeck, von Deuster, Lee & Kozerke (2018). Equilibrated Warping: Finite Element Image Registration with Finite Strain Equilibrium Gap Regularization. Medical Image Analysis, 50, 1–22.]](https://doi.org/10.1016/j.media.2018.07.007).
 ### Requirements
 You need a working installation of FEniCS (including DOLFIN python interface) & VTK (also including python interface).
 ### Installation
 ```
 pip install dolfin_warp
 ```
+### Tutorials
+Interactive tutorials can be found at https://mgenet.gitlabpages.inria.fr/dolfin_warp-tutorials/index.html.
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `dolfin_warp-2023.3.22/dolfin_warp/Energy.py` & `dolfin_warp-2023.5.27/dolfin_warp/Energy.py`

 * *Files identical despite different names*

### Comparing `dolfin_warp-2023.3.22/dolfin_warp/Energy_Continuous.py` & `dolfin_warp-2023.5.27/dolfin_warp/Energy_Continuous.py`

 * *Files identical despite different names*

### Comparing `dolfin_warp-2023.3.22/dolfin_warp/Energy_Continuous_GeneratedImage.py` & `dolfin_warp-2023.5.27/dolfin_warp/Energy_Continuous_GeneratedImage.py`

 * *Files identical despite different names*

### Comparing `dolfin_warp-2023.3.22/dolfin_warp/Energy_Continuous_Regularization.py` & `dolfin_warp-2023.5.27/dolfin_warp/Energy_Continuous_Regularization.py`

 * *Files identical despite different names*

### Comparing `dolfin_warp-2023.3.22/dolfin_warp/Energy_Continuous_WarpedImage.py` & `dolfin_warp-2023.5.27/dolfin_warp/Energy_Continuous_WarpedImage.py`

 * *Files identical despite different names*

### Comparing `dolfin_warp-2023.3.22/dolfin_warp/Energy_Discrete.py` & `dolfin_warp-2023.5.27/dolfin_warp/Energy_Discrete.py`

 * *Files identical despite different names*

### Comparing `dolfin_warp-2023.3.22/dolfin_warp/Energy_Discrete_SimpleRegularization.py` & `dolfin_warp-2023.5.27/dolfin_warp/Energy_Discrete_SimpleRegularization.py`

 * *Files identical despite different names*

### Comparing `dolfin_warp-2023.3.22/dolfin_warp/Energy_Discrete_SurfaceRegularization.py` & `dolfin_warp-2023.5.27/dolfin_warp/Energy_Discrete_SurfaceRegularization.py`

 * *Files identical despite different names*

### Comparing `dolfin_warp-2023.3.22/dolfin_warp/Energy_Discrete_VolumeRegularization.py` & `dolfin_warp-2023.5.27/dolfin_warp/Energy_Discrete_VolumeRegularization.py`

 * *Files identical despite different names*

### Comparing `dolfin_warp-2023.3.22/dolfin_warp/FilesSeries.py` & `dolfin_warp-2023.5.27/dolfin_warp/FilesSeries.py`

 * *Files identical despite different names*

### Comparing `dolfin_warp-2023.3.22/dolfin_warp/FilesSeries_Images.py` & `dolfin_warp-2023.5.27/dolfin_warp/FilesSeries_Images.py`

 * *Files identical despite different names*

### Comparing `dolfin_warp-2023.3.22/dolfin_warp/FilesSeries_Meshes.py` & `dolfin_warp-2023.5.27/dolfin_warp/FilesSeries_Meshes.py`

 * *Files identical despite different names*

### Comparing `dolfin_warp-2023.3.22/dolfin_warp/ImageIterator.py` & `dolfin_warp-2023.5.27/dolfin_warp/ImageIterator.py`

 * *Files identical despite different names*

### Comparing `dolfin_warp-2023.3.22/dolfin_warp/ModalAnalysis.py` & `dolfin_warp-2023.5.27/dolfin_warp/ModalAnalysis.py`

 * *Files identical despite different names*

### Comparing `dolfin_warp-2023.3.22/dolfin_warp/MotionModel.py` & `dolfin_warp-2023.5.27/dolfin_warp/MotionModel.py`

 * *Files identical despite different names*

### Comparing `dolfin_warp-2023.3.22/dolfin_warp/NonlinearSolver.py` & `dolfin_warp-2023.5.27/dolfin_warp/NonlinearSolver.py`

 * *Files identical despite different names*

### Comparing `dolfin_warp-2023.3.22/dolfin_warp/NonlinearSolver_CMA.py` & `dolfin_warp-2023.5.27/dolfin_warp/NonlinearSolver_CMA.py`

 * *Files identical despite different names*

### Comparing `dolfin_warp-2023.3.22/dolfin_warp/NonlinearSolver_Newton.py` & `dolfin_warp-2023.5.27/dolfin_warp/NonlinearSolver_Newton.py`

 * *Files identical despite different names*

### Comparing `dolfin_warp-2023.3.22/dolfin_warp/NonlinearSolver_ReducedKinematicsNewton.py` & `dolfin_warp-2023.5.27/dolfin_warp/NonlinearSolver_ReducedKinematicsNewton.py`

 * *Files identical despite different names*

### Comparing `dolfin_warp-2023.3.22/dolfin_warp/NonlinearSolver_Relaxation.py` & `dolfin_warp-2023.5.27/dolfin_warp/NonlinearSolver_Relaxation.py`

 * *Files 1% similar despite different names*

```diff
@@ -34,15 +34,15 @@
             self.compute_relax = self.compute_relax_aitken
         elif (self.relax_type == "backtracking"):
             self.compute_relax = self.compute_relax_backtracking
             self.relax_backtracking_factor = parameters["relax_backtracking_factor"] if ("relax_backtracking_factor" in parameters) and (parameters["relax_backtracking_factor"] is not None) else 2.
             self.relax_n_iter_max          = parameters["relax_n_iter_max"]          if ("relax_n_iter_max"          in parameters) and (parameters["relax_n_iter_max"]          is not None) else 8
         elif (self.relax_type == "gss"):
             self.compute_relax = self.compute_relax_gss
-            self.relax_n_iter_max   = parameters["relax_n_iter_max"]   if ("relax_n_iter_max"   in parameters) and (parameters["relax_n_iter_max"]   is not None) else 9
+            self.relax_n_iter_max   = parameters["relax_n_iter_max"]   if ("relax_n_iter_max"   in parameters) and (parameters["relax_n_iter_max"]   is not None) else 16
             # self.relax_tol          = parameters["relax_tol"]          if ("relax_tol"          in parameters) and (parameters["relax_tol"]          is not None) else 0
             # self.relax_must_advance = parameters["relax_must_advance"] if ("relax_must_advance" in parameters) and (parameters["relax_must_advance"] is not None) else False
 
 
 
     def compute_relax_constant(self):
 
@@ -59,39 +59,37 @@
             self.relax *= (-1.) * self.res_old_vec.inner(self.dres_vec) / self.dres_norm**2
         self.printer.print_sci("relax",self.relax)
 
 
 
     def compute_relax_backtracking(self):
 
-        relax = 0.
+        relax = 0.; relax_cur = relax
         ener0 = self.problem.assemble_ener()
         self.printer.print_sci("ener0",ener0)
-        relax_cur = 0.
         self.printer.inc()
         k_relax = 1
         while (True):
             self.printer.print_var("k_relax",k_relax,-1)
             relax = 1./self.relax_backtracking_factor**(k_relax-1)
             self.printer.print_sci("relax",relax)
-            self.problem.U.vector().axpy(relax-relax_cur, self.problem.dU.vector())
+            self.problem.U.vector().axpy(relax-relax_cur, self.problem.dU.vector()); relax_cur = relax
             ener = self.problem.assemble_ener()
             self.printer.print_sci("ener",ener)
-            relax_cur = relax
             if (ener < ener0):
                 self.relax = relax
                 break
             if (k_relax == self.relax_n_iter_max):
                 self.relax = 0.
                 self.printer.print_str("Warning! Optimal relaxation is null…")
                 break
             k_relax += 1
         self.printer.dec()
         relax = 0.
-        self.problem.U.vector().axpy(relax-relax_cur, self.problem.dU.vector())
+        self.problem.U.vector().axpy(relax-relax_cur, self.problem.dU.vector()); relax_cur = relax
 
 
 
     def compute_relax_gss(self):
 
         phi = (1 + math.sqrt(5)) / 2
         relax_a = (1-phi)/(2-phi)
```

### Comparing `dolfin_warp-2023.3.22/dolfin_warp/Problem.py` & `dolfin_warp-2023.5.27/dolfin_warp/Problem.py`

 * *Files identical despite different names*

### Comparing `dolfin_warp-2023.3.22/dolfin_warp/Problem_Warping.py` & `dolfin_warp-2023.5.27/dolfin_warp/Problem_Warping.py`

 * *Files identical despite different names*

### Comparing `dolfin_warp-2023.3.22/dolfin_warp/__init__.py` & `dolfin_warp-2023.5.27/dolfin_warp/__init__.py`

 * *Files identical despite different names*

### Comparing `dolfin_warp-2023.3.22/dolfin_warp/compute_best_regularization_strength.py` & `dolfin_warp-2023.5.27/dolfin_warp/compute_best_regularization_strength.py`

 * *Files identical despite different names*

### Comparing `dolfin_warp-2023.3.22/dolfin_warp/compute_displacement_error.py` & `dolfin_warp-2023.5.27/dolfin_warp/compute_displacement_error.py`

 * *Files 20% similar despite different names*

```diff
@@ -4,34 +4,162 @@
 ###                                                                          ###
 ### Created by Martin Genet, 2016-2023                                       ###
 ###                                                                          ###
 ### École Polytechnique, Palaiseau, France                                   ###
 ###                                                                          ###
 ################################################################################
 
+import dolfin
 import numpy
+import vtk
 
 import dolfin_warp as dwarp
 
 ################################################################################
 
+def compute_displacement_error_with_fenics(
+        working_folder          : str                       ,
+        working_basename        : str                       ,
+        ref_folder              : str                       ,
+        ref_basename            : str                       ,
+        working_ext             : str  = "vtu"              ,
+        ref_ext                 : str  = "vtu"              ,
+        working_disp_array_name : str  = "displacement"     ,
+        ref_disp_array_name     : str  = "displacement"     ,
+        suffix                  : str = "displacement_error",
+        sort_mesh               : bool = False              ,
+        verbose                 : bool = True               ):
+
+    assert (sort_mesh == False), "Not implemented in compute_displacement_error_with_fenics, use compute_displacement_error_with_vtk instead. Aborting."
+
+    working_series = dwarp.MeshesSeries(
+        folder   = working_folder  ,
+        basename = working_basename,
+        ext      = working_ext     ,
+        verbose  = verbose         )
+
+    ref_series = dwarp.MeshesSeries(
+        folder   = ref_folder  ,
+        basename = ref_basename,
+        ext      = ref_ext     ,
+        verbose  = verbose     )
+
+    if (ref_series.n_frames != working_series.n_frames):
+        print ("Warning, ref_series.n_frames = "+str(ref_series.n_frames)+" != "+str(working_series.n_frames)+" = working_series.n_frames.")
+    if (verbose): print("n_frames = " + str(working_series.n_frames))
+
+    if (verbose): print("working_zfill = " + str(working_series.zfill))
+    if (verbose): print("ref_zfill     = " + str(ref_series.zfill)    )
+
+    working_mesh_filename  = working_folder
+    working_mesh_filename += "/"+working_basename
+    working_mesh_filename += "-"+"mesh"
+    working_mesh_filename += "."+"xml"
+    working_mesh = dolfin.Mesh(working_mesh_filename)
+    working_fe = dolfin.VectorElement(
+        family="Lagrange",
+        cell=working_mesh.ufl_cell(),
+        degree=1)
+    working_fs = dolfin.FunctionSpace(
+        working_mesh,
+        working_fe)
+    working_U = dolfin.Function(working_fs)
+    working_U.set_allow_extrapolation(True)
+
+    ref_mesh_filename  = ref_folder
+    ref_mesh_filename += "/"+ref_basename
+    ref_mesh_filename += "-"+"mesh"
+    ref_mesh_filename += "."+"xml"
+    ref_mesh = dolfin.Mesh(ref_mesh_filename)
+    ref_mesh_dimension = ref_mesh.ufl_domain().geometric_dimension()
+    ref_mesh_dV = dolfin.Measure("dx", domain=ref_mesh)
+    ref_mesh_V0 = dolfin.assemble(dolfin.Constant(1) * ref_mesh_dV)
+    ref_fe = dolfin.VectorElement(
+        family="Lagrange",
+        cell=ref_mesh.ufl_cell(),
+        degree=1)
+    ref_fs = dolfin.FunctionSpace(
+        ref_mesh,
+        ref_fe)
+    ref_U = dolfin.Function(ref_fs)
+    ref_U.set_allow_extrapolation(True)
+    pro_U = dolfin.Function(ref_fs)
+    pro_U.set_allow_extrapolation(True)
+    err = pro_U - ref_U
+
+    error_file = open(working_folder+"/"+working_basename+"-"+suffix+".dat", "w")
+    error_file.write("#k_frame err_int ref_int sol_int\n")
+
+    err_int = numpy.empty(working_series.n_frames)
+    ref_int = numpy.empty(working_series.n_frames)
+    sol_int = numpy.empty(working_series.n_frames)
+    for k_frame in range(working_series.n_frames):
+        if (verbose): print("k_frame = " + str(k_frame))
+
+        working_ugrid = working_series.get_mesh(k_frame=k_frame)
+        working_array_U = working_ugrid.GetPointData().GetArray(working_disp_array_name)
+        working_array_U = vtk.util.numpy_support.vtk_to_numpy(working_array_U)
+        working_array_U = working_array_U[:,:ref_mesh_dimension]
+        working_array_U = numpy.reshape(working_array_U, working_array_U.size)
+        working_U.vector()[:] = working_array_U
+
+        sol_int[k_frame] = (dolfin.assemble(dolfin.inner(working_U, working_U) * ref_mesh_dV)/ref_mesh_V0)**(0.5)
+        if (verbose): print("sol_int[k_frame] = " + str(sol_int[k_frame]))
+
+        ref_ugrid = ref_series.get_mesh(k_frame=k_frame)
+        ref_array_U = ref_ugrid.GetPointData().GetArray(ref_disp_array_name)
+        ref_array_U = vtk.util.numpy_support.vtk_to_numpy(ref_array_U)
+        ref_array_U = ref_array_U[:,:ref_mesh_dimension]
+        ref_array_U = numpy.reshape(ref_array_U, ref_array_U.size)
+        ref_U.vector()[:] = ref_array_U
+
+        ref_int[k_frame] = (dolfin.assemble(dolfin.inner(ref_U, ref_U) * ref_mesh_dV)/ref_mesh_V0)**(0.5)
+        if (verbose): print("ref_int[k_frame] = " + str(ref_int[k_frame]))
+
+        dolfin.project(
+            v=working_U,
+            V=ref_fs,
+            function=pro_U)
+        if (verbose): print("pro_int = " + str((dolfin.assemble(dolfin.inner(pro_U, pro_U) * ref_mesh_dV)/ref_mesh_V0)**(0.5)))
+
+        err_int[k_frame] = (dolfin.assemble(dolfin.inner(err, err) * ref_mesh_dV)/ref_mesh_V0)**(0.5)
+        if (verbose): print("err_int[k_frame] = " + str(err_int[k_frame]))
+
+    error_file.write("\n".join([" ".join([str(val) for val in [k_frame, err_int[k_frame], ref_int[k_frame], sol_int[k_frame]]]) for k_frame in range(working_series.n_frames)]))
+
+    err_int_int = numpy.sqrt(numpy.mean(numpy.square(err_int)))
+    ref_int_int = numpy.sqrt(numpy.mean(numpy.square(ref_int)))
+    if (verbose): print(err_int_int)
+    if (verbose): print(ref_int_int)
+
+    # error_file.write("\n\n")
+    # error_file.write(" ".join([str(val) for val in [err_int_int, ref_int_int]]))
+
+    error_file.close()
+
+    err = err_int_int/ref_int_int
+    if (verbose): print(err)
+    return err
+
+
+
 def compute_displacement_error_with_numpy(
         working_folder          : str                       ,
         working_basename        : str                       ,
         ref_folder              : str                       ,
         ref_basename            : str                       ,
         working_ext             : str  = "vtu"              ,
         ref_ext                 : str  = "vtu"              ,
         working_disp_array_name : str  = "displacement"     ,
         ref_disp_array_name     : str  = "displacement"     ,
         suffix                  : str = "displacement_error",
         sort_mesh               : bool = False              ,
         verbose                 : bool = True               ):
 
-    assert (sort_mesh == False), "Not implemented in compute_displacement_error_with_numpy, Use compute_displacement_error_with_vtk instead. Aborting."
+    assert (sort_mesh == False), "Not implemented in compute_displacement_error_with_numpy, use compute_displacement_error_with_vtk instead. Aborting."
 
     working_series = dwarp.MeshesSeries(
         folder   = working_folder  ,
         basename = working_basename,
         ext      = working_ext     ,
         verbose  = verbose         )
```

### Comparing `dolfin_warp-2023.3.22/dolfin_warp/compute_displacement_error_field.py` & `dolfin_warp-2023.5.27/dolfin_warp/compute_displacement_error_field.py`

 * *Files identical despite different names*

### Comparing `dolfin_warp-2023.3.22/dolfin_warp/compute_displacement_infinity_norm.py` & `dolfin_warp-2023.5.27/dolfin_warp/compute_displacement_infinity_norm.py`

 * *Files identical despite different names*

### Comparing `dolfin_warp-2023.3.22/dolfin_warp/compute_displacements_from_ref.py` & `dolfin_warp-2023.5.27/dolfin_warp/compute_displacements_from_ref.py`

 * *Files identical despite different names*

### Comparing `dolfin_warp-2023.3.22/dolfin_warp/compute_downsampled_images.py` & `dolfin_warp-2023.5.27/dolfin_warp/compute_downsampled_images.py`

 * *Files identical despite different names*

### Comparing `dolfin_warp-2023.3.22/dolfin_warp/compute_energies_normalization.py` & `dolfin_warp-2023.5.27/dolfin_warp/compute_energies_normalization.py`

 * *Files identical despite different names*

### Comparing `dolfin_warp-2023.3.22/dolfin_warp/compute_equalized_images.py` & `dolfin_warp-2023.5.27/dolfin_warp/compute_equalized_images.py`

 * *Files identical despite different names*

### Comparing `dolfin_warp-2023.3.22/dolfin_warp/compute_normalized_images.py` & `dolfin_warp-2023.5.27/dolfin_warp/compute_normalized_images.py`

 * *Files identical despite different names*

### Comparing `dolfin_warp-2023.3.22/dolfin_warp/compute_projected_image.py` & `dolfin_warp-2023.5.27/dolfin_warp/compute_projected_image.py`

 * *Files identical despite different names*

### Comparing `dolfin_warp-2023.3.22/dolfin_warp/compute_quadrature_degree.py` & `dolfin_warp-2023.5.27/dolfin_warp/compute_quadrature_degree.py`

 * *Files identical despite different names*

### Comparing `dolfin_warp-2023.3.22/dolfin_warp/compute_regularization_energies.py` & `dolfin_warp-2023.5.27/dolfin_warp/compute_regularization_energies.py`

 * *Files identical despite different names*

### Comparing `dolfin_warp-2023.3.22/dolfin_warp/compute_selective_image_gradient.py` & `dolfin_warp-2023.5.27/dolfin_warp/compute_selective_image_gradient.py`

 * *Files identical despite different names*

### Comparing `dolfin_warp-2023.3.22/dolfin_warp/compute_strain_error.py` & `dolfin_warp-2023.5.27/dolfin_warp/compute_strain_error.py`

 * *Files identical despite different names*

### Comparing `dolfin_warp-2023.3.22/dolfin_warp/compute_strains.py` & `dolfin_warp-2023.5.27/dolfin_warp/compute_strains.py`

 * *Files identical despite different names*

### Comparing `dolfin_warp-2023.3.22/dolfin_warp/compute_unwarped_images.py` & `dolfin_warp-2023.5.27/dolfin_warp/compute_unwarped_images.py`

 * *Files identical despite different names*

### Comparing `dolfin_warp-2023.3.22/dolfin_warp/compute_warped_images.py` & `dolfin_warp-2023.5.27/dolfin_warp/compute_warped_images.py`

 * *Files identical despite different names*

### Comparing `dolfin_warp-2023.3.22/dolfin_warp/compute_warped_mesh.py` & `dolfin_warp-2023.5.27/dolfin_warp/compute_warped_mesh.py`

 * *Files identical despite different names*

### Comparing `dolfin_warp-2023.3.22/dolfin_warp/expressions_char_func_cpp.py` & `dolfin_warp-2023.5.27/dolfin_warp/expressions_char_func_cpp.py`

 * *Files identical despite different names*

### Comparing `dolfin_warp-2023.3.22/dolfin_warp/expressions_generated_images_cpp.py` & `dolfin_warp-2023.5.27/dolfin_warp/expressions_generated_images_cpp.py`

 * *Files identical despite different names*

### Comparing `dolfin_warp-2023.3.22/dolfin_warp/expressions_images_cpp.py` & `dolfin_warp-2023.5.27/dolfin_warp/expressions_images_cpp.py`

 * *Files identical despite different names*

### Comparing `dolfin_warp-2023.3.22/dolfin_warp/expressions_images_py.py` & `dolfin_warp-2023.5.27/dolfin_warp/expressions_images_py.py`

 * *Files identical despite different names*

### Comparing `dolfin_warp-2023.3.22/dolfin_warp/expressions_static_scaling_cpp.py` & `dolfin_warp-2023.5.27/dolfin_warp/expressions_static_scaling_cpp.py`

 * *Files identical despite different names*

### Comparing `dolfin_warp-2023.3.22/dolfin_warp/generate_images.py` & `dolfin_warp-2023.5.27/dolfin_warp/generate_images.py`

 * *Files identical despite different names*

### Comparing `dolfin_warp-2023.3.22/dolfin_warp/generate_images_Image.py` & `dolfin_warp-2023.5.27/dolfin_warp/generate_images_Image.py`

 * *Files identical despite different names*

### Comparing `dolfin_warp-2023.3.22/dolfin_warp/generate_images_Mapping.py` & `dolfin_warp-2023.5.27/dolfin_warp/generate_images_Mapping.py`

 * *Files identical despite different names*

### Comparing `dolfin_warp-2023.3.22/dolfin_warp/generate_images_Noise.py` & `dolfin_warp-2023.5.27/dolfin_warp/generate_images_Noise.py`

 * *Files identical despite different names*

### Comparing `dolfin_warp-2023.3.22/dolfin_warp/generate_undersampled_images.py` & `dolfin_warp-2023.5.27/dolfin_warp/generate_undersampled_images.py`

 * *Files identical despite different names*

### Comparing `dolfin_warp-2023.3.22/dolfin_warp/get_centroids.py` & `dolfin_warp-2023.5.27/dolfin_warp/get_centroids.py`

 * *Files identical despite different names*

### Comparing `dolfin_warp-2023.3.22/dolfin_warp/plot_binned_strains_vs_radius.py` & `dolfin_warp-2023.5.27/dolfin_warp/plot_binned_strains_vs_radius.py`

 * *Files identical despite different names*

### Comparing `dolfin_warp-2023.3.22/dolfin_warp/plot_displacement_error.py` & `dolfin_warp-2023.5.27/dolfin_warp/plot_displacement_error.py`

 * *Files identical despite different names*

### Comparing `dolfin_warp-2023.3.22/dolfin_warp/plot_regional_strains.py` & `dolfin_warp-2023.5.27/dolfin_warp/plot_regional_strains.py`

 * *Files identical despite different names*

### Comparing `dolfin_warp-2023.3.22/dolfin_warp/plot_strains.py` & `dolfin_warp-2023.5.27/dolfin_warp/plot_strains.py`

 * *Files identical despite different names*

### Comparing `dolfin_warp-2023.3.22/dolfin_warp/plot_strains_vs_radius.py` & `dolfin_warp-2023.5.27/dolfin_warp/plot_strains_vs_radius.py`

 * *Files identical despite different names*

### Comparing `dolfin_warp-2023.3.22/dolfin_warp/plot_twist_vs_height.py` & `dolfin_warp-2023.5.27/dolfin_warp/plot_twist_vs_height.py`

 * *Files identical despite different names*

### Comparing `dolfin_warp-2023.3.22/dolfin_warp/warp.py` & `dolfin_warp-2023.5.27/dolfin_warp/warp.py`

 * *Files identical despite different names*

### Comparing `dolfin_warp-2023.3.22/dolfin_warp/warp_and_refine.py` & `dolfin_warp-2023.5.27/dolfin_warp/warp_and_refine.py`

 * *Files identical despite different names*

### Comparing `dolfin_warp-2023.3.22/dolfin_warp.egg-info/SOURCES.txt` & `dolfin_warp-2023.5.27/dolfin_warp.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dolfin_warp-2023.3.22/setup.py` & `dolfin_warp-2023.5.27/setup.py`

 * *Files identical despite different names*

