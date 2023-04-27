# Comparing `tmp/mplsoccer-1.1.8.tar.gz` & `tmp/mplsoccer-1.1.9.tar.gz`

## Comparing `mplsoccer-1.1.8.tar` & `mplsoccer-1.1.9.tar`

### file list

```diff
@@ -1,104 +1,104 @@
--rw-r--r--   0        0        0    20213 2020-02-02 00:00:00.000000 mplsoccer-1.1.8/.pylintrc
--rw-r--r--   0        0        0      451 2020-02-02 00:00:00.000000 mplsoccer-1.1.8/.readthedocs.yml
--rw-r--r--   0        0        0    22240 2020-02-02 00:00:00.000000 mplsoccer-1.1.8/CHANGELOG.md
--rw-r--r--   0        0        0      387 2020-02-02 00:00:00.000000 mplsoccer-1.1.8/environment-dev.yml
--rw-r--r--   0        0        0      323 2020-02-02 00:00:00.000000 mplsoccer-1.1.8/environment-docs.yml
--rw-r--r--   0        0        0      263 2020-02-02 00:00:00.000000 mplsoccer-1.1.8/environment.yml
--rw-r--r--   0        0        0       53 2020-02-02 00:00:00.000000 mplsoccer-1.1.8/requirements.txt
--rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 mplsoccer-1.1.8/docs/Makefile
--rw-r--r--   0        0        0      799 2020-02-02 00:00:00.000000 mplsoccer-1.1.8/docs/make.bat
--rw-r--r--   0        0        0   385285 2020-02-02 00:00:00.000000 mplsoccer-1.1.8/docs/quick_start.png
--rw-r--r--   0        0        0    56598 2020-02-02 00:00:00.000000 mplsoccer-1.1.8/docs/quick_start_radar.png
--rw-r--r--   0        0        0    63145 2020-02-02 00:00:00.000000 mplsoccer-1.1.8/docs/source/Mplsoccer logo github.jpg
--rw-r--r--   0        0        0      238 2020-02-02 00:00:00.000000 mplsoccer-1.1.8/docs/source/api.rst
--rw-r--r--   0        0        0     3921 2020-02-02 00:00:00.000000 mplsoccer-1.1.8/docs/source/conf.py
--rw-r--r--   0        0        0   138151 2020-02-02 00:00:00.000000 mplsoccer-1.1.8/docs/source/explain_standardizer.png
--rw-r--r--   0        0        0     2880 2020-02-02 00:00:00.000000 mplsoccer-1.1.8/docs/source/index.rst
--rw-r--r--   0        0        0      223 2020-02-02 00:00:00.000000 mplsoccer-1.1.8/docs/source/installation.rst
--rw-r--r--   0        0        0    93798 2020-02-02 00:00:00.000000 mplsoccer-1.1.8/docs/source/logo-white.png
--rw-r--r--   0        0        0   123658 2020-02-02 00:00:00.000000 mplsoccer-1.1.8/docs/source/logo.png
--rw-r--r--   0        0        0      151 2020-02-02 00:00:00.000000 mplsoccer-1.1.8/docs/source/mplsoccer.bumpy_chart.rst
--rw-r--r--   0        0        0      134 2020-02-02 00:00:00.000000 mplsoccer-1.1.8/docs/source/mplsoccer.grid.rst
--rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 mplsoccer-1.1.8/docs/source/mplsoccer.linecollection.rst
--rw-r--r--   0        0        0      156 2020-02-02 00:00:00.000000 mplsoccer-1.1.8/docs/source/mplsoccer.pitch.rst
--rw-r--r--   0        0        0      142 2020-02-02 00:00:00.000000 mplsoccer-1.1.8/docs/source/mplsoccer.py_pizza.rst
--rw-r--r--   0        0        0      136 2020-02-02 00:00:00.000000 mplsoccer-1.1.8/docs/source/mplsoccer.quiver.rst
--rw-r--r--   0        0        0      151 2020-02-02 00:00:00.000000 mplsoccer-1.1.8/docs/source/mplsoccer.radar_chart.rst
--rw-r--r--   0        0        0      145 2020-02-02 00:00:00.000000 mplsoccer-1.1.8/docs/source/mplsoccer.statsbomb.rst
--rw-r--r--   0        0        0      137 2020-02-02 00:00:00.000000 mplsoccer-1.1.8/docs/source/mplsoccer.utils.rst
--rw-r--r--   0        0        0      621 2020-02-02 00:00:00.000000 mplsoccer-1.1.8/examples/README.rst
--rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 mplsoccer-1.1.8/examples/bumpy_charts/README.rst
--rw-r--r--   0        0        0    10499 2020-02-02 00:00:00.000000 mplsoccer-1.1.8/examples/bumpy_charts/plot_bumpy.py
--rw-r--r--   0        0        0       84 2020-02-02 00:00:00.000000 mplsoccer-1.1.8/examples/pitch_plots/README.rst
--rw-r--r--   0        0        0     5303 2020-02-02 00:00:00.000000 mplsoccer-1.1.8/examples/pitch_plots/plot_animation.py
--rw-r--r--   0        0        0     4062 2020-02-02 00:00:00.000000 mplsoccer-1.1.8/examples/pitch_plots/plot_arrows.py
--rw-r--r--   0        0        0    10554 2020-02-02 00:00:00.000000 mplsoccer-1.1.8/examples/pitch_plots/plot_cmap.py
--rw-r--r--   0        0        0     1010 2020-02-02 00:00:00.000000 mplsoccer-1.1.8/examples/pitch_plots/plot_convex_hull.py
--rw-r--r--   0        0        0     4144 2020-02-02 00:00:00.000000 mplsoccer-1.1.8/examples/pitch_plots/plot_cyberpunk.py
--rw-r--r--   0        0        0     1781 2020-02-02 00:00:00.000000 mplsoccer-1.1.8/examples/pitch_plots/plot_delaunay.py
--rw-r--r--   0        0        0     7933 2020-02-02 00:00:00.000000 mplsoccer-1.1.8/examples/pitch_plots/plot_fbref.py
--rw-r--r--   0        0        0     5410 2020-02-02 00:00:00.000000 mplsoccer-1.1.8/examples/pitch_plots/plot_flow.py
--rw-r--r--   0        0        0    16017 2020-02-02 00:00:00.000000 mplsoccer-1.1.8/examples/pitch_plots/plot_grid.py
--rw-r--r--   0        0        0    10158 2020-02-02 00:00:00.000000 mplsoccer-1.1.8/examples/pitch_plots/plot_heatmap.py
--rw-r--r--   0        0        0     3990 2020-02-02 00:00:00.000000 mplsoccer-1.1.8/examples/pitch_plots/plot_heatmap_positional.py
--rw-r--r--   0        0        0     6477 2020-02-02 00:00:00.000000 mplsoccer-1.1.8/examples/pitch_plots/plot_hexbin.py
--rw-r--r--   0        0        0    18384 2020-02-02 00:00:00.000000 mplsoccer-1.1.8/examples/pitch_plots/plot_jointgrid.py
--rw-r--r--   0        0        0     7200 2020-02-02 00:00:00.000000 mplsoccer-1.1.8/examples/pitch_plots/plot_kde.py
--rw-r--r--   0        0        0     6644 2020-02-02 00:00:00.000000 mplsoccer-1.1.8/examples/pitch_plots/plot_lines.py
--rw-r--r--   0        0        0     9458 2020-02-02 00:00:00.000000 mplsoccer-1.1.8/examples/pitch_plots/plot_pass_network.py
--rw-r--r--   0        0        0     3344 2020-02-02 00:00:00.000000 mplsoccer-1.1.8/examples/pitch_plots/plot_photo.py
--rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 mplsoccer-1.1.8/examples/pitch_plots/plot_sb360_frame.py
--rw-r--r--   0        0        0    18274 2020-02-02 00:00:00.000000 mplsoccer-1.1.8/examples/pitch_plots/plot_scatter.py
--rw-r--r--   0        0        0     3969 2020-02-02 00:00:00.000000 mplsoccer-1.1.8/examples/pitch_plots/plot_shot_freeze_frame.py
--rw-r--r--   0        0        0    11528 2020-02-02 00:00:00.000000 mplsoccer-1.1.8/examples/pitch_plots/plot_standardize.py
--rw-r--r--   0        0        0     1233 2020-02-02 00:00:00.000000 mplsoccer-1.1.8/examples/pitch_plots/plot_textured_background.py
--rw-r--r--   0        0        0     7942 2020-02-02 00:00:00.000000 mplsoccer-1.1.8/examples/pitch_plots/plot_twitter_powerpoint.py
--rw-r--r--   0        0        0     1720 2020-02-02 00:00:00.000000 mplsoccer-1.1.8/examples/pitch_plots/plot_voronoi.py
--rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 mplsoccer-1.1.8/examples/pitch_setup/README.rst
--rw-r--r--   0        0        0     3377 2020-02-02 00:00:00.000000 mplsoccer-1.1.8/examples/pitch_setup/plot_compare_pitches.py
--rw-r--r--   0        0        0    14142 2020-02-02 00:00:00.000000 mplsoccer-1.1.8/examples/pitch_setup/plot_explain_standardizer.py
--rw-r--r--   0        0        0     8554 2020-02-02 00:00:00.000000 mplsoccer-1.1.8/examples/pitch_setup/plot_pitches.py
--rw-r--r--   0        0        0      926 2020-02-02 00:00:00.000000 mplsoccer-1.1.8/examples/pitch_setup/plot_quick_start.py
--rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 mplsoccer-1.1.8/examples/pizza_plots/README.rst
--rw-r--r--   0        0        0    12084 2020-02-02 00:00:00.000000 mplsoccer-1.1.8/examples/pizza_plots/plot_pizza_basic.py
--rw-r--r--   0        0        0     5803 2020-02-02 00:00:00.000000 mplsoccer-1.1.8/examples/pizza_plots/plot_pizza_colorful.py
--rw-r--r--   0        0        0     8787 2020-02-02 00:00:00.000000 mplsoccer-1.1.8/examples/pizza_plots/plot_pizza_comparison.py
--rw-r--r--   0        0        0     9332 2020-02-02 00:00:00.000000 mplsoccer-1.1.8/examples/pizza_plots/plot_pizza_comparison_vary_scales.py
--rw-r--r--   0        0        0     5812 2020-02-02 00:00:00.000000 mplsoccer-1.1.8/examples/pizza_plots/plot_pizza_dark_theme.py
--rw-r--r--   0        0        0     3845 2020-02-02 00:00:00.000000 mplsoccer-1.1.8/examples/pizza_plots/plot_pizza_different_units.py
--rw-r--r--   0        0        0     5173 2020-02-02 00:00:00.000000 mplsoccer-1.1.8/examples/pizza_plots/plot_pizza_scales_vary.py
--rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 mplsoccer-1.1.8/examples/radar/README.rst
--rw-r--r--   0        0        0    23909 2020-02-02 00:00:00.000000 mplsoccer-1.1.8/examples/radar/plot_radar.py
--rw-r--r--   0        0        0     8903 2020-02-02 00:00:00.000000 mplsoccer-1.1.8/examples/radar/plot_turbine.py
--rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 mplsoccer-1.1.8/examples/statsbomb/README.rst
--rw-r--r--   0        0        0     2719 2020-02-02 00:00:00.000000 mplsoccer-1.1.8/examples/statsbomb/plot_statsbomb_data.py
--rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 mplsoccer-1.1.8/examples/tutorials/README.rst
--rw-r--r--   0        0        0     1934 2020-02-02 00:00:00.000000 mplsoccer-1.1.8/examples/tutorials/plot_wedges.py
--rw-r--r--   0        0        0    11296 2020-02-02 00:00:00.000000 mplsoccer-1.1.8/examples/tutorials/plot_xt.py
--rw-r--r--   0        0        0     9766 2020-02-02 00:00:00.000000 mplsoccer-1.1.8/examples/tutorials/plot_xt_improvements.py
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 mplsoccer-1.1.8/mplsoccer/__about__.py
--rw-r--r--   0        0        0      440 2020-02-02 00:00:00.000000 mplsoccer-1.1.8/mplsoccer/__init__.py
--rw-r--r--   0        0        0    52979 2020-02-02 00:00:00.000000 mplsoccer-1.1.8/mplsoccer/_pitch_base.py
--rw-r--r--   0        0        0    33672 2020-02-02 00:00:00.000000 mplsoccer-1.1.8/mplsoccer/_pitch_plot.py
--rw-r--r--   0        0        0    11518 2020-02-02 00:00:00.000000 mplsoccer-1.1.8/mplsoccer/bumpy_chart.py
--rw-r--r--   0        0        0     2306 2020-02-02 00:00:00.000000 mplsoccer-1.1.8/mplsoccer/cm.py
--rw-r--r--   0        0        0    19708 2020-02-02 00:00:00.000000 mplsoccer-1.1.8/mplsoccer/dimensions.py
--rw-r--r--   0        0        0    14933 2020-02-02 00:00:00.000000 mplsoccer-1.1.8/mplsoccer/grid.py
--rw-r--r--   0        0        0    15704 2020-02-02 00:00:00.000000 mplsoccer-1.1.8/mplsoccer/heatmap.py
--rw-r--r--   0        0        0    10644 2020-02-02 00:00:00.000000 mplsoccer-1.1.8/mplsoccer/linecollection.py
--rw-r--r--   0        0        0     9864 2020-02-02 00:00:00.000000 mplsoccer-1.1.8/mplsoccer/pitch.py
--rw-r--r--   0        0        0    21880 2020-02-02 00:00:00.000000 mplsoccer-1.1.8/mplsoccer/py_pizza.py
--rw-r--r--   0        0        0     6133 2020-02-02 00:00:00.000000 mplsoccer-1.1.8/mplsoccer/quiver.py
--rw-r--r--   0        0        0    34817 2020-02-02 00:00:00.000000 mplsoccer-1.1.8/mplsoccer/radar_chart.py
--rw-r--r--   0        0        0    19156 2020-02-02 00:00:00.000000 mplsoccer-1.1.8/mplsoccer/scatterutils.py
--rw-r--r--   0        0        0    24921 2020-02-02 00:00:00.000000 mplsoccer-1.1.8/mplsoccer/statsbomb.py
--rw-r--r--   0        0        0    11926 2020-02-02 00:00:00.000000 mplsoccer-1.1.8/mplsoccer/utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mplsoccer-1.1.8/tests/__init__.py
--rw-r--r--   0        0        0     4221 2020-02-02 00:00:00.000000 mplsoccer-1.1.8/tests/test_bin_statistic.py
--rw-r--r--   0        0        0     1647 2020-02-02 00:00:00.000000 mplsoccer-1.1.8/tests/test_grid.py
--rw-r--r--   0        0        0     3126 2020-02-02 00:00:00.000000 mplsoccer-1.1.8/tests/test_standarizer.py
--rw-r--r--   0        0        0     2325 2020-02-02 00:00:00.000000 mplsoccer-1.1.8/.gitignore
--rw-r--r--   0        0        0     1088 2020-02-02 00:00:00.000000 mplsoccer-1.1.8/LICENSE
--rw-r--r--   0        0        0     3464 2020-02-02 00:00:00.000000 mplsoccer-1.1.8/README.md
--rw-r--r--   0        0        0     1864 2020-02-02 00:00:00.000000 mplsoccer-1.1.8/pyproject.toml
--rw-r--r--   0        0        0     4665 2020-02-02 00:00:00.000000 mplsoccer-1.1.8/PKG-INFO
+-rw-r--r--   0        0        0    20213 2020-02-02 00:00:00.000000 mplsoccer-1.1.9/.pylintrc
+-rw-r--r--   0        0        0      451 2020-02-02 00:00:00.000000 mplsoccer-1.1.9/.readthedocs.yml
+-rw-r--r--   0        0        0    22411 2020-02-02 00:00:00.000000 mplsoccer-1.1.9/CHANGELOG.md
+-rw-r--r--   0        0        0      387 2020-02-02 00:00:00.000000 mplsoccer-1.1.9/environment-dev.yml
+-rw-r--r--   0        0        0      323 2020-02-02 00:00:00.000000 mplsoccer-1.1.9/environment-docs.yml
+-rw-r--r--   0        0        0      263 2020-02-02 00:00:00.000000 mplsoccer-1.1.9/environment.yml
+-rw-r--r--   0        0        0       53 2020-02-02 00:00:00.000000 mplsoccer-1.1.9/requirements.txt
+-rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 mplsoccer-1.1.9/docs/Makefile
+-rw-r--r--   0        0        0      799 2020-02-02 00:00:00.000000 mplsoccer-1.1.9/docs/make.bat
+-rw-r--r--   0        0        0   385285 2020-02-02 00:00:00.000000 mplsoccer-1.1.9/docs/quick_start.png
+-rw-r--r--   0        0        0    56598 2020-02-02 00:00:00.000000 mplsoccer-1.1.9/docs/quick_start_radar.png
+-rw-r--r--   0        0        0    63145 2020-02-02 00:00:00.000000 mplsoccer-1.1.9/docs/source/Mplsoccer logo github.jpg
+-rw-r--r--   0        0        0      238 2020-02-02 00:00:00.000000 mplsoccer-1.1.9/docs/source/api.rst
+-rw-r--r--   0        0        0     3921 2020-02-02 00:00:00.000000 mplsoccer-1.1.9/docs/source/conf.py
+-rw-r--r--   0        0        0   138151 2020-02-02 00:00:00.000000 mplsoccer-1.1.9/docs/source/explain_standardizer.png
+-rw-r--r--   0        0        0     2880 2020-02-02 00:00:00.000000 mplsoccer-1.1.9/docs/source/index.rst
+-rw-r--r--   0        0        0      223 2020-02-02 00:00:00.000000 mplsoccer-1.1.9/docs/source/installation.rst
+-rw-r--r--   0        0        0    93798 2020-02-02 00:00:00.000000 mplsoccer-1.1.9/docs/source/logo-white.png
+-rw-r--r--   0        0        0   123658 2020-02-02 00:00:00.000000 mplsoccer-1.1.9/docs/source/logo.png
+-rw-r--r--   0        0        0      151 2020-02-02 00:00:00.000000 mplsoccer-1.1.9/docs/source/mplsoccer.bumpy_chart.rst
+-rw-r--r--   0        0        0      134 2020-02-02 00:00:00.000000 mplsoccer-1.1.9/docs/source/mplsoccer.grid.rst
+-rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 mplsoccer-1.1.9/docs/source/mplsoccer.linecollection.rst
+-rw-r--r--   0        0        0      156 2020-02-02 00:00:00.000000 mplsoccer-1.1.9/docs/source/mplsoccer.pitch.rst
+-rw-r--r--   0        0        0      142 2020-02-02 00:00:00.000000 mplsoccer-1.1.9/docs/source/mplsoccer.py_pizza.rst
+-rw-r--r--   0        0        0      136 2020-02-02 00:00:00.000000 mplsoccer-1.1.9/docs/source/mplsoccer.quiver.rst
+-rw-r--r--   0        0        0      151 2020-02-02 00:00:00.000000 mplsoccer-1.1.9/docs/source/mplsoccer.radar_chart.rst
+-rw-r--r--   0        0        0      145 2020-02-02 00:00:00.000000 mplsoccer-1.1.9/docs/source/mplsoccer.statsbomb.rst
+-rw-r--r--   0        0        0      137 2020-02-02 00:00:00.000000 mplsoccer-1.1.9/docs/source/mplsoccer.utils.rst
+-rw-r--r--   0        0        0      621 2020-02-02 00:00:00.000000 mplsoccer-1.1.9/examples/README.rst
+-rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 mplsoccer-1.1.9/examples/bumpy_charts/README.rst
+-rw-r--r--   0        0        0    10499 2020-02-02 00:00:00.000000 mplsoccer-1.1.9/examples/bumpy_charts/plot_bumpy.py
+-rw-r--r--   0        0        0       84 2020-02-02 00:00:00.000000 mplsoccer-1.1.9/examples/pitch_plots/README.rst
+-rw-r--r--   0        0        0     5303 2020-02-02 00:00:00.000000 mplsoccer-1.1.9/examples/pitch_plots/plot_animation.py
+-rw-r--r--   0        0        0     4062 2020-02-02 00:00:00.000000 mplsoccer-1.1.9/examples/pitch_plots/plot_arrows.py
+-rw-r--r--   0        0        0    10554 2020-02-02 00:00:00.000000 mplsoccer-1.1.9/examples/pitch_plots/plot_cmap.py
+-rw-r--r--   0        0        0     1010 2020-02-02 00:00:00.000000 mplsoccer-1.1.9/examples/pitch_plots/plot_convex_hull.py
+-rw-r--r--   0        0        0     4144 2020-02-02 00:00:00.000000 mplsoccer-1.1.9/examples/pitch_plots/plot_cyberpunk.py
+-rw-r--r--   0        0        0     1781 2020-02-02 00:00:00.000000 mplsoccer-1.1.9/examples/pitch_plots/plot_delaunay.py
+-rw-r--r--   0        0        0     7952 2020-02-02 00:00:00.000000 mplsoccer-1.1.9/examples/pitch_plots/plot_fbref.py
+-rw-r--r--   0        0        0     5410 2020-02-02 00:00:00.000000 mplsoccer-1.1.9/examples/pitch_plots/plot_flow.py
+-rw-r--r--   0        0        0    16017 2020-02-02 00:00:00.000000 mplsoccer-1.1.9/examples/pitch_plots/plot_grid.py
+-rw-r--r--   0        0        0    10158 2020-02-02 00:00:00.000000 mplsoccer-1.1.9/examples/pitch_plots/plot_heatmap.py
+-rw-r--r--   0        0        0     3990 2020-02-02 00:00:00.000000 mplsoccer-1.1.9/examples/pitch_plots/plot_heatmap_positional.py
+-rw-r--r--   0        0        0     6477 2020-02-02 00:00:00.000000 mplsoccer-1.1.9/examples/pitch_plots/plot_hexbin.py
+-rw-r--r--   0        0        0    18384 2020-02-02 00:00:00.000000 mplsoccer-1.1.9/examples/pitch_plots/plot_jointgrid.py
+-rw-r--r--   0        0        0     7200 2020-02-02 00:00:00.000000 mplsoccer-1.1.9/examples/pitch_plots/plot_kde.py
+-rw-r--r--   0        0        0     6644 2020-02-02 00:00:00.000000 mplsoccer-1.1.9/examples/pitch_plots/plot_lines.py
+-rw-r--r--   0        0        0     9458 2020-02-02 00:00:00.000000 mplsoccer-1.1.9/examples/pitch_plots/plot_pass_network.py
+-rw-r--r--   0        0        0     3344 2020-02-02 00:00:00.000000 mplsoccer-1.1.9/examples/pitch_plots/plot_photo.py
+-rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 mplsoccer-1.1.9/examples/pitch_plots/plot_sb360_frame.py
+-rw-r--r--   0        0        0    18274 2020-02-02 00:00:00.000000 mplsoccer-1.1.9/examples/pitch_plots/plot_scatter.py
+-rw-r--r--   0        0        0     3969 2020-02-02 00:00:00.000000 mplsoccer-1.1.9/examples/pitch_plots/plot_shot_freeze_frame.py
+-rw-r--r--   0        0        0    11528 2020-02-02 00:00:00.000000 mplsoccer-1.1.9/examples/pitch_plots/plot_standardize.py
+-rw-r--r--   0        0        0     1233 2020-02-02 00:00:00.000000 mplsoccer-1.1.9/examples/pitch_plots/plot_textured_background.py
+-rw-r--r--   0        0        0     7942 2020-02-02 00:00:00.000000 mplsoccer-1.1.9/examples/pitch_plots/plot_twitter_powerpoint.py
+-rw-r--r--   0        0        0     1720 2020-02-02 00:00:00.000000 mplsoccer-1.1.9/examples/pitch_plots/plot_voronoi.py
+-rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 mplsoccer-1.1.9/examples/pitch_setup/README.rst
+-rw-r--r--   0        0        0     3377 2020-02-02 00:00:00.000000 mplsoccer-1.1.9/examples/pitch_setup/plot_compare_pitches.py
+-rw-r--r--   0        0        0    14142 2020-02-02 00:00:00.000000 mplsoccer-1.1.9/examples/pitch_setup/plot_explain_standardizer.py
+-rw-r--r--   0        0        0     8554 2020-02-02 00:00:00.000000 mplsoccer-1.1.9/examples/pitch_setup/plot_pitches.py
+-rw-r--r--   0        0        0      926 2020-02-02 00:00:00.000000 mplsoccer-1.1.9/examples/pitch_setup/plot_quick_start.py
+-rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 mplsoccer-1.1.9/examples/pizza_plots/README.rst
+-rw-r--r--   0        0        0    12084 2020-02-02 00:00:00.000000 mplsoccer-1.1.9/examples/pizza_plots/plot_pizza_basic.py
+-rw-r--r--   0        0        0     5803 2020-02-02 00:00:00.000000 mplsoccer-1.1.9/examples/pizza_plots/plot_pizza_colorful.py
+-rw-r--r--   0        0        0     8787 2020-02-02 00:00:00.000000 mplsoccer-1.1.9/examples/pizza_plots/plot_pizza_comparison.py
+-rw-r--r--   0        0        0     9332 2020-02-02 00:00:00.000000 mplsoccer-1.1.9/examples/pizza_plots/plot_pizza_comparison_vary_scales.py
+-rw-r--r--   0        0        0     5812 2020-02-02 00:00:00.000000 mplsoccer-1.1.9/examples/pizza_plots/plot_pizza_dark_theme.py
+-rw-r--r--   0        0        0     3845 2020-02-02 00:00:00.000000 mplsoccer-1.1.9/examples/pizza_plots/plot_pizza_different_units.py
+-rw-r--r--   0        0        0     5173 2020-02-02 00:00:00.000000 mplsoccer-1.1.9/examples/pizza_plots/plot_pizza_scales_vary.py
+-rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 mplsoccer-1.1.9/examples/radar/README.rst
+-rw-r--r--   0        0        0    23909 2020-02-02 00:00:00.000000 mplsoccer-1.1.9/examples/radar/plot_radar.py
+-rw-r--r--   0        0        0     8903 2020-02-02 00:00:00.000000 mplsoccer-1.1.9/examples/radar/plot_turbine.py
+-rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 mplsoccer-1.1.9/examples/statsbomb/README.rst
+-rw-r--r--   0        0        0     2719 2020-02-02 00:00:00.000000 mplsoccer-1.1.9/examples/statsbomb/plot_statsbomb_data.py
+-rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 mplsoccer-1.1.9/examples/tutorials/README.rst
+-rw-r--r--   0        0        0     1934 2020-02-02 00:00:00.000000 mplsoccer-1.1.9/examples/tutorials/plot_wedges.py
+-rw-r--r--   0        0        0    11296 2020-02-02 00:00:00.000000 mplsoccer-1.1.9/examples/tutorials/plot_xt.py
+-rw-r--r--   0        0        0     9766 2020-02-02 00:00:00.000000 mplsoccer-1.1.9/examples/tutorials/plot_xt_improvements.py
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 mplsoccer-1.1.9/mplsoccer/__about__.py
+-rw-r--r--   0        0        0      440 2020-02-02 00:00:00.000000 mplsoccer-1.1.9/mplsoccer/__init__.py
+-rw-r--r--   0        0        0    53400 2020-02-02 00:00:00.000000 mplsoccer-1.1.9/mplsoccer/_pitch_base.py
+-rw-r--r--   0        0        0    33672 2020-02-02 00:00:00.000000 mplsoccer-1.1.9/mplsoccer/_pitch_plot.py
+-rw-r--r--   0        0        0    11518 2020-02-02 00:00:00.000000 mplsoccer-1.1.9/mplsoccer/bumpy_chart.py
+-rw-r--r--   0        0        0     2306 2020-02-02 00:00:00.000000 mplsoccer-1.1.9/mplsoccer/cm.py
+-rw-r--r--   0        0        0    19708 2020-02-02 00:00:00.000000 mplsoccer-1.1.9/mplsoccer/dimensions.py
+-rw-r--r--   0        0        0    14933 2020-02-02 00:00:00.000000 mplsoccer-1.1.9/mplsoccer/grid.py
+-rw-r--r--   0        0        0    15704 2020-02-02 00:00:00.000000 mplsoccer-1.1.9/mplsoccer/heatmap.py
+-rw-r--r--   0        0        0    10644 2020-02-02 00:00:00.000000 mplsoccer-1.1.9/mplsoccer/linecollection.py
+-rw-r--r--   0        0        0     9864 2020-02-02 00:00:00.000000 mplsoccer-1.1.9/mplsoccer/pitch.py
+-rw-r--r--   0        0        0    21880 2020-02-02 00:00:00.000000 mplsoccer-1.1.9/mplsoccer/py_pizza.py
+-rw-r--r--   0        0        0     6133 2020-02-02 00:00:00.000000 mplsoccer-1.1.9/mplsoccer/quiver.py
+-rw-r--r--   0        0        0    34817 2020-02-02 00:00:00.000000 mplsoccer-1.1.9/mplsoccer/radar_chart.py
+-rw-r--r--   0        0        0    19156 2020-02-02 00:00:00.000000 mplsoccer-1.1.9/mplsoccer/scatterutils.py
+-rw-r--r--   0        0        0    24921 2020-02-02 00:00:00.000000 mplsoccer-1.1.9/mplsoccer/statsbomb.py
+-rw-r--r--   0        0        0    11926 2020-02-02 00:00:00.000000 mplsoccer-1.1.9/mplsoccer/utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mplsoccer-1.1.9/tests/__init__.py
+-rw-r--r--   0        0        0     4221 2020-02-02 00:00:00.000000 mplsoccer-1.1.9/tests/test_bin_statistic.py
+-rw-r--r--   0        0        0     1647 2020-02-02 00:00:00.000000 mplsoccer-1.1.9/tests/test_grid.py
+-rw-r--r--   0        0        0     3126 2020-02-02 00:00:00.000000 mplsoccer-1.1.9/tests/test_standarizer.py
+-rw-r--r--   0        0        0     2325 2020-02-02 00:00:00.000000 mplsoccer-1.1.9/.gitignore
+-rw-r--r--   0        0        0     1088 2020-02-02 00:00:00.000000 mplsoccer-1.1.9/LICENSE
+-rw-r--r--   0        0        0     3464 2020-02-02 00:00:00.000000 mplsoccer-1.1.9/README.md
+-rw-r--r--   0        0        0     1864 2020-02-02 00:00:00.000000 mplsoccer-1.1.9/pyproject.toml
+-rw-r--r--   0        0        0     4665 2020-02-02 00:00:00.000000 mplsoccer-1.1.9/PKG-INFO
```

### Comparing `mplsoccer-1.1.8/.pylintrc` & `mplsoccer-1.1.9/.pylintrc`

 * *Files identical despite different names*

### Comparing `mplsoccer-1.1.8/CHANGELOG.md` & `mplsoccer-1.1.9/CHANGELOG.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,14 @@
+:rocket: Version 1.1.9
+----------------------
+
+### Fixes
+* Fixed positional pitch marking to remove extraneous lines when ``Pitch`` is created with 
+``positional=True`` 
+
 :rocket: Version 1.1.8
 ----------------------
 
 ### Fixes
 * Fixed goal width dimensions for ``opta_dims`` definitions from (44.62,55.38) to (45.2,54.8)
 
 :rocket: Version 1.1.7
```

### Comparing `mplsoccer-1.1.8/docs/Makefile` & `mplsoccer-1.1.9/docs/Makefile`

 * *Files identical despite different names*

### Comparing `mplsoccer-1.1.8/docs/make.bat` & `mplsoccer-1.1.9/docs/make.bat`

 * *Files identical despite different names*

### Comparing `mplsoccer-1.1.8/docs/quick_start.png` & `mplsoccer-1.1.9/docs/quick_start.png`

 * *Files identical despite different names*

### Comparing `mplsoccer-1.1.8/docs/quick_start_radar.png` & `mplsoccer-1.1.9/docs/quick_start_radar.png`

 * *Files identical despite different names*

### Comparing `mplsoccer-1.1.8/docs/source/Mplsoccer logo github.jpg` & `mplsoccer-1.1.9/docs/source/Mplsoccer logo github.jpg`

 * *Files identical despite different names*

### Comparing `mplsoccer-1.1.8/docs/source/conf.py` & `mplsoccer-1.1.9/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `mplsoccer-1.1.8/docs/source/explain_standardizer.png` & `mplsoccer-1.1.9/docs/source/explain_standardizer.png`

 * *Files identical despite different names*

### Comparing `mplsoccer-1.1.8/docs/source/index.rst` & `mplsoccer-1.1.9/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `mplsoccer-1.1.8/docs/source/logo-white.png` & `mplsoccer-1.1.9/docs/source/logo-white.png`

 * *Files identical despite different names*

### Comparing `mplsoccer-1.1.8/docs/source/logo.png` & `mplsoccer-1.1.9/docs/source/logo.png`

 * *Files identical despite different names*

### Comparing `mplsoccer-1.1.8/examples/README.rst` & `mplsoccer-1.1.9/examples/README.rst`

 * *Files identical despite different names*

### Comparing `mplsoccer-1.1.8/examples/bumpy_charts/plot_bumpy.py` & `mplsoccer-1.1.9/examples/bumpy_charts/plot_bumpy.py`

 * *Files identical despite different names*

### Comparing `mplsoccer-1.1.8/examples/pitch_plots/plot_animation.py` & `mplsoccer-1.1.9/examples/pitch_plots/plot_animation.py`

 * *Files identical despite different names*

### Comparing `mplsoccer-1.1.8/examples/pitch_plots/plot_arrows.py` & `mplsoccer-1.1.9/examples/pitch_plots/plot_arrows.py`

 * *Files identical despite different names*

### Comparing `mplsoccer-1.1.8/examples/pitch_plots/plot_cmap.py` & `mplsoccer-1.1.9/examples/pitch_plots/plot_cmap.py`

 * *Files identical despite different names*

### Comparing `mplsoccer-1.1.8/examples/pitch_plots/plot_convex_hull.py` & `mplsoccer-1.1.9/examples/pitch_plots/plot_convex_hull.py`

 * *Files identical despite different names*

### Comparing `mplsoccer-1.1.8/examples/pitch_plots/plot_cyberpunk.py` & `mplsoccer-1.1.9/examples/pitch_plots/plot_cyberpunk.py`

 * *Files identical despite different names*

### Comparing `mplsoccer-1.1.8/examples/pitch_plots/plot_delaunay.py` & `mplsoccer-1.1.9/examples/pitch_plots/plot_delaunay.py`

 * *Files identical despite different names*

### Comparing `mplsoccer-1.1.8/examples/pitch_plots/plot_fbref.py` & `mplsoccer-1.1.9/examples/pitch_plots/plot_fbref.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
 ==============
-FBRef Pressure
+FBRef Touches
 ==============
 
-This example shows how to scrape pressure events from FBRef.com and plot them as a heatmap.
+This example shows how to scrape touches events from FBRef.com and plot them as a heatmap.
 """
 from urllib.request import urlopen
 
 import matplotlib.patheffects as path_effects
 import matplotlib.pyplot as plt
 import pandas as pd
 from PIL import Image
@@ -15,53 +15,53 @@
 from mplsoccer import Pitch, FontManager, add_image
 
 ##############################################################################
 # Scrape the data via a link to a specific table.
 # To get the link for a different league,
 # find the table you want from the website. Then click "Share & more" and copy the link from
 # the option "Modify & Share Table". Then "click url for sharing" and get the table as a url.
-URL = 'https://fbref.com/en/share/eDK2O'
+URL = 'https://fbref.com/en/share/LdLSY'
 df = pd.read_html(URL)[0]
-# select a subset of the columns (Squad and pressure columns)
-df = df[['Unnamed: 0_level_0', 'Pressures']].copy()
+# select a subset of the columns (Squad and touches columns)
+df = df[['Unnamed: 0_level_0', 'Touches']].copy()
 df.columns = df.columns.droplevel()  # drop the top-level of the multi-index
+df = df.drop(["Def Pen", "Att Pen", "Live"], axis = 1) # drop the def pen, att pen, live touches column
 
 ##############################################################################
 # Get the league average percentages
-pressure_cols = ['Def 3rd', 'Mid 3rd', 'Att 3rd']
-df_total = pd.DataFrame(df[pressure_cols].sum())
+touches_cols = ['Def 3rd', 'Mid 3rd', 'Att 3rd']
+df_total = pd.DataFrame(df[touches_cols].sum())
 df_total.columns = ['total']
 df_total = df_total.T
 df_total = df_total.divide(df_total.sum(axis=1), axis=0) * 100
 
 ##############################################################################
-# Calculate the percentages for each team and sort so that the teams which press higher are last
-df[pressure_cols] = df[pressure_cols].divide(df[pressure_cols].sum(axis=1), axis=0) * 100.
+# Calculate the percentages for each team and sort so that the teams make the most touches are last
+df[touches_cols] = df[touches_cols].divide(df[touches_cols].sum(axis=1), axis=0) * 100.
 df.sort_values(['Att 3rd', 'Def 3rd'], ascending=[True, False], inplace=True)
 
 ##############################################################################
-# Get the StatsBomb logo and Fonts
+# Get Stats Perform's logo and Fonts
 
-SB_LOGO_URL = ('https://raw.githubusercontent.com/statsbomb/open-data/'
-               'master/img/SB%20-%20Icon%20Lockup%20-%20Colour%20positive.png')
-sb_logo = Image.open(urlopen(SB_LOGO_URL))
+SP_LOGO_URL = ('https://upload.wikimedia.org/wikipedia/commons/d/d5/StatsPerform_Logo_Primary_01.png')
+sp_logo = Image.open(urlopen(SP_LOGO_URL))
 
 # a FontManager object for using a google font (default Robotto)
 fm = FontManager()
 # path effects
 path_eff = [path_effects.Stroke(linewidth=3, foreground='black'),
             path_effects.Normal()]
 
 ##############################################################################
 # Plot the percentages
 
 # setup a mplsoccer pitch
 pitch = Pitch(line_zorder=2, line_color='black', pad_top=20)
 
-# mplsoccer calculates the binned statistics usually from raw locations, such as pressure events
+# mplsoccer calculates the binned statistics usually from raw locations, such as touches events
 # for this example we will create a binned statistic dividing
 # the pitch into thirds for one point (0, 0)
 # we will fill this in a loop later with each team's statistics from the dataframe
 bin_statistic = pitch.bin_statistic([0], [0], statistic='count', bins=(3, 1))
 
 GRID_HEIGHT = 0.8
 CBAR_WIDTH = 0.03
@@ -72,25 +72,25 @@
                       # Turn off the endnote/title axis. I usually do this after
                       # I am happy with the chart layout and text placement
                       axis=False,
                       title_space=0.02, title_height=0.06, grid_height=GRID_HEIGHT)
 fig.set_facecolor('white')
 
 teams = df['Squad'].values
-vmin = df[pressure_cols].min().min()  # we normalise the heatmaps with the min / max values
-vmax = df[pressure_cols].max().max()
+vmin = df[touches_cols].min().min()  # we normalise the heatmaps with the min / max values
+vmax = df[touches_cols].max().max()
 for i, ax in enumerate(axs['pitch'].flat[:len(teams)]):
-    # the top of the StatsBomb pitch is zero
+    # the top of the pitch is zero
     # plot the title half way between zero and -20 (the top padding)
     ax.text(60, -10, teams[i],
             ha='center', va='center', fontsize=50,
             fontproperties=fm.prop)
 
     # fill in the bin statistics from df and plot the heatmap
-    bin_statistic['statistic'] = df.loc[df.Squad == teams[i], pressure_cols].values
+    bin_statistic['statistic'] = df.loc[df.Squad == teams[i], touches_cols].values
     heatmap = pitch.heatmap(bin_statistic, ax=ax, cmap='coolwarm', vmin=vmin, vmax=vmax)
     annotate = pitch.label_heatmap(bin_statistic, color='white', fontproperties=fm.prop,
                                    path_effects=path_eff, fontsize=50, ax=ax,
                                    str_format='{0:.0f}%', ha='center', va='center')
 
 # if its the Bundesliga remove the two spare pitches
 if len(teams) == 18:
@@ -105,49 +105,49 @@
                         GRID_HEIGHT - 0.036))
 cbar = plt.colorbar(heatmap, cax=ax_cbar)
 for label in cbar.ax.get_yticklabels():
     label.set_fontproperties(fm.prop)
     label.set_fontsize(50)
 
 # title and endnote
-add_image(sb_logo, fig,
+add_image(sp_logo, fig,
           left=axs['endnote'].get_position().x0,
           bottom=axs['endnote'].get_position().y0,
           height=axs['endnote'].get_position().height)
-title = axs['title'].text(0.5, 0.5, 'Pressure events %, Bundesliga, 2019/20',
+title = axs['title'].text(0.5, 0.5, 'Touches events %, Bundesliga, 2022/23',
                           ha='center', va='center', fontsize=70)
 
 ##############################################################################
 # Plot the percentage point difference
 
 # Calculate the percentage point difference from the league average
-df[pressure_cols] = df[pressure_cols].values - df_total.values
+df[touches_cols] = df[touches_cols].values - df_total.values
 
 GRID_HEIGHT = 0.76
 fig, axs = pitch.grid(nrows=4, ncols=5, figheight=20,
                       # leaves some space on the right hand side for the colorbar
                       grid_width=0.88, left=0.025,
                       endnote_height=0.03, endnote_space=0,
                       # Turn off the endnote/title axis. I usually do this after
                       # I am happy with the chart layout and text placement
                       axis=False,
                       title_space=0.02, title_height=0.1, grid_height=GRID_HEIGHT)
 fig.set_facecolor('white')
 
 teams = df['Squad'].values
-vmin = df[pressure_cols].min().min()  # we normalise the heatmaps with the min / max values
-vmax = df[pressure_cols].max().max()
+vmin = df[touches_cols].min().min()  # we normalise the heatmaps with the min / max values
+vmax = df[touches_cols].max().max()
 
 for i, ax in enumerate(axs['pitch'].flat[:len(teams)]):
-    # the top of the StatsBomb pitch is zero
+    # the top of the pitch is zero
     # plot the title half way between zero and -20 (the top padding)
     ax.text(60, -10, teams[i], ha='center', va='center', fontsize=50, fontproperties=fm.prop)
 
     # fill in the bin statistics from df and plot the heatmap
-    bin_statistic['statistic'] = df.loc[df.Squad == teams[i], pressure_cols].values
+    bin_statistic['statistic'] = df.loc[df.Squad == teams[i], touches_cols].values
     heatmap = pitch.heatmap(bin_statistic, ax=ax, cmap='coolwarm', vmin=vmin, vmax=vmax)
     annotate = pitch.label_heatmap(bin_statistic, color='white', fontproperties=fm.prop,
                                    path_effects=path_eff, str_format='{0:.0f}%', fontsize=50,
                                    ax=ax, ha='center', va='center')
 
 # if its the Bundesliga remove the two spare pitches
 if len(teams) == 18:
@@ -162,15 +162,15 @@
                         GRID_HEIGHT - 0.035))
 cbar = plt.colorbar(heatmap, cax=ax_cbar)
 for label in cbar.ax.get_yticklabels():
     label.set_fontproperties(fm.prop)
     label.set_fontsize(50)
 
 # title and endnote
-add_image(sb_logo, fig,
+add_image(sp_logo, fig,
           left=axs['endnote'].get_position().x0,
           bottom=axs['endnote'].get_position().y0,
           height=axs['endnote'].get_position().height)
-TITLE = 'Pressure events, percentage point difference\nfrom the Bundesliga average 2019/20'
+TITLE = 'Touches events, percentage point difference\nfrom the Bundesliga average 2022/23'
 title = axs['title'].text(0.5, 0.5, TITLE, ha='center', va='center', fontsize=60)
 
 plt.show()  # If you are using a Jupyter notebook you do not need this line
```

### Comparing `mplsoccer-1.1.8/examples/pitch_plots/plot_flow.py` & `mplsoccer-1.1.9/examples/pitch_plots/plot_flow.py`

 * *Files identical despite different names*

### Comparing `mplsoccer-1.1.8/examples/pitch_plots/plot_grid.py` & `mplsoccer-1.1.9/examples/pitch_plots/plot_grid.py`

 * *Files identical despite different names*

### Comparing `mplsoccer-1.1.8/examples/pitch_plots/plot_heatmap.py` & `mplsoccer-1.1.9/examples/pitch_plots/plot_heatmap.py`

 * *Files identical despite different names*

### Comparing `mplsoccer-1.1.8/examples/pitch_plots/plot_heatmap_positional.py` & `mplsoccer-1.1.9/examples/pitch_plots/plot_heatmap_positional.py`

 * *Files identical despite different names*

### Comparing `mplsoccer-1.1.8/examples/pitch_plots/plot_hexbin.py` & `mplsoccer-1.1.9/examples/pitch_plots/plot_hexbin.py`

 * *Files identical despite different names*

### Comparing `mplsoccer-1.1.8/examples/pitch_plots/plot_jointgrid.py` & `mplsoccer-1.1.9/examples/pitch_plots/plot_jointgrid.py`

 * *Files identical despite different names*

### Comparing `mplsoccer-1.1.8/examples/pitch_plots/plot_kde.py` & `mplsoccer-1.1.9/examples/pitch_plots/plot_kde.py`

 * *Files identical despite different names*

### Comparing `mplsoccer-1.1.8/examples/pitch_plots/plot_lines.py` & `mplsoccer-1.1.9/examples/pitch_plots/plot_lines.py`

 * *Files identical despite different names*

### Comparing `mplsoccer-1.1.8/examples/pitch_plots/plot_pass_network.py` & `mplsoccer-1.1.9/examples/pitch_plots/plot_pass_network.py`

 * *Files identical despite different names*

### Comparing `mplsoccer-1.1.8/examples/pitch_plots/plot_photo.py` & `mplsoccer-1.1.9/examples/pitch_plots/plot_photo.py`

 * *Files identical despite different names*

### Comparing `mplsoccer-1.1.8/examples/pitch_plots/plot_sb360_frame.py` & `mplsoccer-1.1.9/examples/pitch_plots/plot_sb360_frame.py`

 * *Files identical despite different names*

### Comparing `mplsoccer-1.1.8/examples/pitch_plots/plot_scatter.py` & `mplsoccer-1.1.9/examples/pitch_plots/plot_scatter.py`

 * *Files identical despite different names*

### Comparing `mplsoccer-1.1.8/examples/pitch_plots/plot_shot_freeze_frame.py` & `mplsoccer-1.1.9/examples/pitch_plots/plot_shot_freeze_frame.py`

 * *Files identical despite different names*

### Comparing `mplsoccer-1.1.8/examples/pitch_plots/plot_standardize.py` & `mplsoccer-1.1.9/examples/pitch_plots/plot_standardize.py`

 * *Files identical despite different names*

### Comparing `mplsoccer-1.1.8/examples/pitch_plots/plot_textured_background.py` & `mplsoccer-1.1.9/examples/pitch_plots/plot_textured_background.py`

 * *Files identical despite different names*

### Comparing `mplsoccer-1.1.8/examples/pitch_plots/plot_twitter_powerpoint.py` & `mplsoccer-1.1.9/examples/pitch_plots/plot_twitter_powerpoint.py`

 * *Files identical despite different names*

### Comparing `mplsoccer-1.1.8/examples/pitch_plots/plot_voronoi.py` & `mplsoccer-1.1.9/examples/pitch_plots/plot_voronoi.py`

 * *Files identical despite different names*

### Comparing `mplsoccer-1.1.8/examples/pitch_setup/plot_compare_pitches.py` & `mplsoccer-1.1.9/examples/pitch_setup/plot_compare_pitches.py`

 * *Files identical despite different names*

### Comparing `mplsoccer-1.1.8/examples/pitch_setup/plot_explain_standardizer.py` & `mplsoccer-1.1.9/examples/pitch_setup/plot_explain_standardizer.py`

 * *Files identical despite different names*

### Comparing `mplsoccer-1.1.8/examples/pitch_setup/plot_pitches.py` & `mplsoccer-1.1.9/examples/pitch_setup/plot_pitches.py`

 * *Files identical despite different names*

### Comparing `mplsoccer-1.1.8/examples/pitch_setup/plot_quick_start.py` & `mplsoccer-1.1.9/examples/pitch_setup/plot_quick_start.py`

 * *Files identical despite different names*

### Comparing `mplsoccer-1.1.8/examples/pizza_plots/plot_pizza_basic.py` & `mplsoccer-1.1.9/examples/pizza_plots/plot_pizza_basic.py`

 * *Files identical despite different names*

### Comparing `mplsoccer-1.1.8/examples/pizza_plots/plot_pizza_colorful.py` & `mplsoccer-1.1.9/examples/pizza_plots/plot_pizza_colorful.py`

 * *Files identical despite different names*

### Comparing `mplsoccer-1.1.8/examples/pizza_plots/plot_pizza_comparison.py` & `mplsoccer-1.1.9/examples/pizza_plots/plot_pizza_comparison.py`

 * *Files identical despite different names*

### Comparing `mplsoccer-1.1.8/examples/pizza_plots/plot_pizza_comparison_vary_scales.py` & `mplsoccer-1.1.9/examples/pizza_plots/plot_pizza_comparison_vary_scales.py`

 * *Files identical despite different names*

### Comparing `mplsoccer-1.1.8/examples/pizza_plots/plot_pizza_dark_theme.py` & `mplsoccer-1.1.9/examples/pizza_plots/plot_pizza_dark_theme.py`

 * *Files identical despite different names*

### Comparing `mplsoccer-1.1.8/examples/pizza_plots/plot_pizza_different_units.py` & `mplsoccer-1.1.9/examples/pizza_plots/plot_pizza_different_units.py`

 * *Files identical despite different names*

### Comparing `mplsoccer-1.1.8/examples/pizza_plots/plot_pizza_scales_vary.py` & `mplsoccer-1.1.9/examples/pizza_plots/plot_pizza_scales_vary.py`

 * *Files identical despite different names*

### Comparing `mplsoccer-1.1.8/examples/radar/plot_radar.py` & `mplsoccer-1.1.9/examples/radar/plot_radar.py`

 * *Files identical despite different names*

### Comparing `mplsoccer-1.1.8/examples/radar/plot_turbine.py` & `mplsoccer-1.1.9/examples/radar/plot_turbine.py`

 * *Files identical despite different names*

### Comparing `mplsoccer-1.1.8/examples/statsbomb/plot_statsbomb_data.py` & `mplsoccer-1.1.9/examples/statsbomb/plot_statsbomb_data.py`

 * *Files identical despite different names*

### Comparing `mplsoccer-1.1.8/examples/tutorials/plot_wedges.py` & `mplsoccer-1.1.9/examples/tutorials/plot_wedges.py`

 * *Files identical despite different names*

### Comparing `mplsoccer-1.1.8/examples/tutorials/plot_xt.py` & `mplsoccer-1.1.9/examples/tutorials/plot_xt.py`

 * *Files identical despite different names*

### Comparing `mplsoccer-1.1.8/examples/tutorials/plot_xt_improvements.py` & `mplsoccer-1.1.9/examples/tutorials/plot_xt_improvements.py`

 * *Files identical despite different names*

### Comparing `mplsoccer-1.1.8/mplsoccer/_pitch_base.py` & `mplsoccer-1.1.9/mplsoccer/_pitch_base.py`

 * *Files 2% similar despite different names*

```diff
@@ -593,16 +593,21 @@
                                    zorder=self.line_zorder)
 
     def _draw_juego_de_posicion(self, ax):
         line_prop = {'linewidth': self.positional_linewidth, 'color': self.positional_color,
                      'alpha': self.line_alpha, 'linestyle': self.positional_linestyle,
                      'zorder': self.positional_zorder}
         # x lines for Juego de Posición
-        for coord in self.dim.positional_x[1:-1]:
-            self._draw_line(ax, [coord, coord], [self.dim.bottom, self.dim.top], **line_prop)
+        #through lines
+        self._draw_line(ax, [self.dim.positional_x[1], self.dim.positional_x[1]], [self.dim.bottom, self.dim.top], **line_prop)
+        self._draw_line(ax, [self.dim.positional_x[5], self.dim.positional_x[5]], [self.dim.bottom, self.dim.top], **line_prop)
+        #short lines
+        for coord in self.dim.positional_x[2:5]:
+            self._draw_line(ax, [coord, coord], [self.dim.bottom,  self.dim.penalty_area_bottom], **line_prop)
+            self._draw_line(ax, [coord, coord], [self.dim.top,  self.dim.penalty_area_top], **line_prop)
         # y lines for Juego de Posición
         self._draw_line(ax, [self.dim.left, self.dim.right],
                         [self.dim.positional_y[1], self.dim.positional_y[1]], **line_prop)
         self._draw_line(ax, [self.dim.penalty_area_left, self.dim.penalty_area_right],
                         [self.dim.positional_y[2], self.dim.positional_y[2]], **line_prop)
         self._draw_line(ax, [self.dim.penalty_area_left, self.dim.penalty_area_right],
                         [self.dim.positional_y[3], self.dim.positional_y[3]], **line_prop)
```

### Comparing `mplsoccer-1.1.8/mplsoccer/_pitch_plot.py` & `mplsoccer-1.1.9/mplsoccer/_pitch_plot.py`

 * *Files identical despite different names*

### Comparing `mplsoccer-1.1.8/mplsoccer/bumpy_chart.py` & `mplsoccer-1.1.9/mplsoccer/bumpy_chart.py`

 * *Files identical despite different names*

### Comparing `mplsoccer-1.1.8/mplsoccer/cm.py` & `mplsoccer-1.1.9/mplsoccer/cm.py`

 * *Files identical despite different names*

### Comparing `mplsoccer-1.1.8/mplsoccer/dimensions.py` & `mplsoccer-1.1.9/mplsoccer/dimensions.py`

 * *Files identical despite different names*

### Comparing `mplsoccer-1.1.8/mplsoccer/grid.py` & `mplsoccer-1.1.9/mplsoccer/grid.py`

 * *Files identical despite different names*

### Comparing `mplsoccer-1.1.8/mplsoccer/heatmap.py` & `mplsoccer-1.1.9/mplsoccer/heatmap.py`

 * *Files identical despite different names*

### Comparing `mplsoccer-1.1.8/mplsoccer/linecollection.py` & `mplsoccer-1.1.9/mplsoccer/linecollection.py`

 * *Files identical despite different names*

### Comparing `mplsoccer-1.1.8/mplsoccer/pitch.py` & `mplsoccer-1.1.9/mplsoccer/pitch.py`

 * *Files identical despite different names*

### Comparing `mplsoccer-1.1.8/mplsoccer/py_pizza.py` & `mplsoccer-1.1.9/mplsoccer/py_pizza.py`

 * *Files identical despite different names*

### Comparing `mplsoccer-1.1.8/mplsoccer/quiver.py` & `mplsoccer-1.1.9/mplsoccer/quiver.py`

 * *Files identical despite different names*

### Comparing `mplsoccer-1.1.8/mplsoccer/radar_chart.py` & `mplsoccer-1.1.9/mplsoccer/radar_chart.py`

 * *Files identical despite different names*

### Comparing `mplsoccer-1.1.8/mplsoccer/scatterutils.py` & `mplsoccer-1.1.9/mplsoccer/scatterutils.py`

 * *Files identical despite different names*

### Comparing `mplsoccer-1.1.8/mplsoccer/statsbomb.py` & `mplsoccer-1.1.9/mplsoccer/statsbomb.py`

 * *Files identical despite different names*

### Comparing `mplsoccer-1.1.8/mplsoccer/utils.py` & `mplsoccer-1.1.9/mplsoccer/utils.py`

 * *Files identical despite different names*

### Comparing `mplsoccer-1.1.8/tests/test_bin_statistic.py` & `mplsoccer-1.1.9/tests/test_bin_statistic.py`

 * *Files identical despite different names*

### Comparing `mplsoccer-1.1.8/tests/test_grid.py` & `mplsoccer-1.1.9/tests/test_grid.py`

 * *Files identical despite different names*

### Comparing `mplsoccer-1.1.8/tests/test_standarizer.py` & `mplsoccer-1.1.9/tests/test_standarizer.py`

 * *Files identical despite different names*

### Comparing `mplsoccer-1.1.8/.gitignore` & `mplsoccer-1.1.9/.gitignore`

 * *Files identical despite different names*

### Comparing `mplsoccer-1.1.8/LICENSE` & `mplsoccer-1.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `mplsoccer-1.1.8/README.md` & `mplsoccer-1.1.9/README.md`

 * *Files identical despite different names*

### Comparing `mplsoccer-1.1.8/pyproject.toml` & `mplsoccer-1.1.9/pyproject.toml`

 * *Files identical despite different names*

### Comparing `mplsoccer-1.1.8/PKG-INFO` & `mplsoccer-1.1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mplsoccer
-Version: 1.1.8
+Version: 1.1.9
 Summary: Football pitch plotting library for matplotlib
 Project-URL: Documentation, https://mplsoccer.readthedocs.io
 Project-URL: Issues, https://github.com/andrewRowlinson/mplsoccer/issues
 Project-URL: Source, https://github.com/andrewRowlinson/mplsoccer
 Author-email: Andrew Rowlinson <rowlinsonandy@gmail.com>, Anmol Durgapal <slothfulwave10@gmail.com>
 License-File: LICENSE
 Keywords: football,matplotlib,mplsoccer,soccer,visualization
```

