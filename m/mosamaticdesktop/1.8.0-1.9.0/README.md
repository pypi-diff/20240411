# Comparing `tmp/mosamaticdesktop-1.8.0.tar.gz` & `tmp/mosamaticdesktop-1.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mosamaticdesktop-1.8.0.tar", last modified: Fri Jan 26 14:35:23 2024, max compression
+gzip compressed data, was "mosamaticdesktop-1.9.0.tar", last modified: Fri Jan 26 17:32:57 2024, max compression
```

## Comparing `mosamaticdesktop-1.8.0.tar` & `mosamaticdesktop-1.9.0.tar`

### file list

```diff
@@ -1,127 +1,135 @@
-drwxr-xr-x   0 Ralph      (501) staff       (20)        0 2024-01-26 14:35:23.967921 mosamaticdesktop-1.8.0/
--rw-r--r--   0 Ralph      (501) staff       (20)      690 2024-01-26 14:35:23.967610 mosamaticdesktop-1.8.0/PKG-INFO
-drwxr-xr-x   0 Ralph      (501) staff       (20)        0 2024-01-26 14:35:23.929281 mosamaticdesktop-1.8.0/mosamaticdesktop/
--rw-r--r--   0 Ralph      (501) staff       (20)        0 2024-01-26 07:38:53.000000 mosamaticdesktop-1.8.0/mosamaticdesktop/__init__.py
-drwxr-xr-x   0 Ralph      (501) staff       (20)        0 2024-01-26 14:35:23.936794 mosamaticdesktop-1.8.0/mosamaticdesktop/ai/
--rw-r--r--   0 Ralph      (501) staff       (20)        0 2024-01-26 07:38:53.000000 mosamaticdesktop-1.8.0/mosamaticdesktop/ai/__init__.py
--rw-r--r--   0 Ralph      (501) staff       (20)      266 2024-01-26 07:38:53.000000 mosamaticdesktop-1.8.0/mosamaticdesktop/ai/model.py
--rw-r--r--   0 Ralph      (501) staff       (20)      432 2024-01-26 07:38:53.000000 mosamaticdesktop-1.8.0/mosamaticdesktop/ai/pytorchmodel.py
--rw-r--r--   0 Ralph      (501) staff       (20)      536 2024-01-26 07:38:53.000000 mosamaticdesktop-1.8.0/mosamaticdesktop/ai/tensorflowmodel.py
-drwxr-xr-x   0 Ralph      (501) staff       (20)        0 2024-01-26 14:35:23.939308 mosamaticdesktop-1.8.0/mosamaticdesktop/data/
--rw-r--r--   0 Ralph      (501) staff       (20)        0 2024-01-26 07:38:53.000000 mosamaticdesktop-1.8.0/mosamaticdesktop/data/__init__.py
--rw-r--r--   0 Ralph      (501) staff       (20)     4446 2024-01-26 07:38:53.000000 mosamaticdesktop-1.8.0/mosamaticdesktop/data/datamanager.py
--rw-r--r--   0 Ralph      (501) staff       (20)      519 2024-01-26 07:38:53.000000 mosamaticdesktop-1.8.0/mosamaticdesktop/data/engine.py
--rw-r--r--   0 Ralph      (501) staff       (20)      374 2024-01-26 07:38:53.000000 mosamaticdesktop-1.8.0/mosamaticdesktop/data/file.py
--rw-r--r--   0 Ralph      (501) staff       (20)      395 2024-01-26 07:38:53.000000 mosamaticdesktop-1.8.0/mosamaticdesktop/data/filecontent.py
--rw-r--r--   0 Ralph      (501) staff       (20)      683 2024-01-26 07:38:53.000000 mosamaticdesktop-1.8.0/mosamaticdesktop/data/filecontentcache.py
--rw-r--r--   0 Ralph      (501) staff       (20)      894 2024-01-26 07:38:53.000000 mosamaticdesktop-1.8.0/mosamaticdesktop/data/fileset.py
-drwxr-xr-x   0 Ralph      (501) staff       (20)        0 2024-01-26 14:35:23.940472 mosamaticdesktop-1.8.0/mosamaticdesktop/data/models/
--rw-r--r--   0 Ralph      (501) staff       (20)        0 2024-01-26 07:38:53.000000 mosamaticdesktop-1.8.0/mosamaticdesktop/data/models/__init__.py
--rw-r--r--   0 Ralph      (501) staff       (20)       87 2024-01-26 07:38:53.000000 mosamaticdesktop-1.8.0/mosamaticdesktop/data/models/basemodel.py
--rw-r--r--   0 Ralph      (501) staff       (20)      715 2024-01-26 07:38:53.000000 mosamaticdesktop-1.8.0/mosamaticdesktop/data/models/filemodel.py
--rw-r--r--   0 Ralph      (501) staff       (20)      724 2024-01-26 07:38:53.000000 mosamaticdesktop-1.8.0/mosamaticdesktop/data/models/filesetmodel.py
--rw-r--r--   0 Ralph      (501) staff       (20)      370 2024-01-26 07:38:53.000000 mosamaticdesktop-1.8.0/mosamaticdesktop/data/session.py
--rw-r--r--   0 Ralph      (501) staff       (20)     2216 2024-01-26 07:38:53.000000 mosamaticdesktop-1.8.0/mosamaticdesktop/logger.py
--rw-r--r--   0 Ralph      (501) staff       (20)      300 2024-01-26 07:38:53.000000 mosamaticdesktop-1.8.0/mosamaticdesktop/main.py
--rw-r--r--   0 Ralph      (501) staff       (20)      266 2024-01-26 07:38:53.000000 mosamaticdesktop-1.8.0/mosamaticdesktop/maintest.py
--rw-r--r--   0 Ralph      (501) staff       (20)     5711 2024-01-26 07:38:53.000000 mosamaticdesktop-1.8.0/mosamaticdesktop/mainwindow.py
--rw-r--r--   0 Ralph      (501) staff       (20)      475 2024-01-26 07:38:53.000000 mosamaticdesktop-1.8.0/mosamaticdesktop/operatingsystem.py
-drwxr-xr-x   0 Ralph      (501) staff       (20)        0 2024-01-26 14:35:23.941772 mosamaticdesktop-1.8.0/mosamaticdesktop/scripts/
--rw-r--r--   0 Ralph      (501) staff       (20)      220 2024-01-26 11:01:32.000000 mosamaticdesktop-1.8.0/mosamaticdesktop/scripts/mosamatic.bat
--rwxr-xr-x   0 Ralph      (501) staff       (20)      135 2024-01-26 11:00:56.000000 mosamaticdesktop-1.8.0/mosamaticdesktop/scripts/mosamatic.sh
--rw-r--r--   0 Ralph      (501) staff       (20)      223 2024-01-26 07:38:53.000000 mosamaticdesktop-1.8.0/mosamaticdesktop/singleton.py
-drwxr-xr-x   0 Ralph      (501) staff       (20)        0 2024-01-26 14:35:23.949151 mosamaticdesktop-1.8.0/mosamaticdesktop/tasks/
--rw-r--r--   0 Ralph      (501) staff       (20)        0 2024-01-26 07:38:53.000000 mosamaticdesktop-1.8.0/mosamaticdesktop/tasks/__init__.py
--rw-r--r--   0 Ralph      (501) staff       (20)     1454 2024-01-26 07:38:53.000000 mosamaticdesktop-1.8.0/mosamaticdesktop/tasks/booleanparameter.py
-drwxr-xr-x   0 Ralph      (501) staff       (20)        0 2024-01-26 14:35:23.950685 mosamaticdesktop-1.8.0/mosamaticdesktop/tasks/calculatebodycompositionmetricstask/
--rw-r--r--   0 Ralph      (501) staff       (20)        0 2024-01-26 07:38:53.000000 mosamaticdesktop-1.8.0/mosamaticdesktop/tasks/calculatebodycompositionmetricstask/__init__.py
--rw-r--r--   0 Ralph      (501) staff       (20)    11453 2024-01-26 14:31:29.000000 mosamaticdesktop-1.8.0/mosamaticdesktop/tasks/calculatebodycompositionmetricstask/calculatebodycompositionmetricstask.py
--rw-r--r--   0 Ralph      (501) staff       (20)     1682 2024-01-26 07:38:53.000000 mosamaticdesktop-1.8.0/mosamaticdesktop/tasks/calculatebodycompositionmetricstask/calculatebodycompositionmetricstaskwidget.py
-drwxr-xr-x   0 Ralph      (501) staff       (20)        0 2024-01-26 14:35:23.951491 mosamaticdesktop-1.8.0/mosamaticdesktop/tasks/checkdicomheadertask/
--rw-r--r--   0 Ralph      (501) staff       (20)        0 2024-01-26 07:38:53.000000 mosamaticdesktop-1.8.0/mosamaticdesktop/tasks/checkdicomheadertask/__init__.py
--rw-r--r--   0 Ralph      (501) staff       (20)     3566 2024-01-26 14:31:21.000000 mosamaticdesktop-1.8.0/mosamaticdesktop/tasks/checkdicomheadertask/checkdicomheadertask.py
--rw-r--r--   0 Ralph      (501) staff       (20)     2345 2024-01-26 07:38:53.000000 mosamaticdesktop-1.8.0/mosamaticdesktop/tasks/checkdicomheadertask/checkdicomheadertaskwidget.py
-drwxr-xr-x   0 Ralph      (501) staff       (20)        0 2024-01-26 14:35:23.952208 mosamaticdesktop-1.8.0/mosamaticdesktop/tasks/copyfilesettask/
--rw-r--r--   0 Ralph      (501) staff       (20)        0 2024-01-26 07:38:53.000000 mosamaticdesktop-1.8.0/mosamaticdesktop/tasks/copyfilesettask/__init__.py
--rw-r--r--   0 Ralph      (501) staff       (20)     1919 2024-01-26 14:31:15.000000 mosamaticdesktop-1.8.0/mosamaticdesktop/tasks/copyfilesettask/copyfilesettask.py
--rw-r--r--   0 Ralph      (501) staff       (20)     1170 2024-01-26 07:38:53.000000 mosamaticdesktop-1.8.0/mosamaticdesktop/tasks/copyfilesettask/copyfilesettaskwidget.py
-drwxr-xr-x   0 Ralph      (501) staff       (20)        0 2024-01-26 14:35:23.953077 mosamaticdesktop-1.8.0/mosamaticdesktop/tasks/createarchivetask/
--rw-r--r--   0 Ralph      (501) staff       (20)        0 2024-01-26 07:38:53.000000 mosamaticdesktop-1.8.0/mosamaticdesktop/tasks/createarchivetask/__init__.py
--rw-r--r--   0 Ralph      (501) staff       (20)     1803 2024-01-26 14:31:09.000000 mosamaticdesktop-1.8.0/mosamaticdesktop/tasks/createarchivetask/createarchivetask.py
--rw-r--r--   0 Ralph      (501) staff       (20)     1157 2024-01-26 07:38:53.000000 mosamaticdesktop-1.8.0/mosamaticdesktop/tasks/createarchivetask/createarchivetaskwidget.py
-drwxr-xr-x   0 Ralph      (501) staff       (20)        0 2024-01-26 14:35:23.953825 mosamaticdesktop-1.8.0/mosamaticdesktop/tasks/createpngfromdicomfiletask/
--rw-r--r--   0 Ralph      (501) staff       (20)        0 2024-01-26 07:38:53.000000 mosamaticdesktop-1.8.0/mosamaticdesktop/tasks/createpngfromdicomfiletask/__init__.py
--rw-r--r--   0 Ralph      (501) staff       (20)     2562 2024-01-26 14:31:03.000000 mosamaticdesktop-1.8.0/mosamaticdesktop/tasks/createpngfromdicomfiletask/createpngfromdicomfiletask.py
--rw-r--r--   0 Ralph      (501) staff       (20)     1633 2024-01-26 07:38:53.000000 mosamaticdesktop-1.8.0/mosamaticdesktop/tasks/createpngfromdicomfiletask/createpngfromdicomfiletaskwidget.py
-drwxr-xr-x   0 Ralph      (501) staff       (20)        0 2024-01-26 14:35:23.955131 mosamaticdesktop-1.8.0/mosamaticdesktop/tasks/createpngfromsegmentationfiletask/
--rw-r--r--   0 Ralph      (501) staff       (20)        0 2024-01-26 07:38:53.000000 mosamaticdesktop-1.8.0/mosamaticdesktop/tasks/createpngfromsegmentationfiletask/__init__.py
--rw-r--r--   0 Ralph      (501) staff       (20)     2369 2024-01-26 14:30:05.000000 mosamaticdesktop-1.8.0/mosamaticdesktop/tasks/createpngfromsegmentationfiletask/createpngfromsegmentationfiletask.py
--rw-r--r--   0 Ralph      (501) staff       (20)     1236 2024-01-26 14:30:47.000000 mosamaticdesktop-1.8.0/mosamaticdesktop/tasks/createpngfromsegmentationfiletask/createpngfromsegmentationfiletaskwidget.py
-drwxr-xr-x   0 Ralph      (501) staff       (20)        0 2024-01-26 14:35:23.956083 mosamaticdesktop-1.8.0/mosamaticdesktop/tasks/createpngfromtagfiletask/
--rw-r--r--   0 Ralph      (501) staff       (20)        0 2024-01-26 07:38:53.000000 mosamaticdesktop-1.8.0/mosamaticdesktop/tasks/createpngfromtagfiletask/__init__.py
--rw-r--r--   0 Ralph      (501) staff       (20)     2312 2024-01-26 14:29:38.000000 mosamaticdesktop-1.8.0/mosamaticdesktop/tasks/createpngfromtagfiletask/createpngfromtagfiletask.py
--rw-r--r--   0 Ralph      (501) staff       (20)     1194 2024-01-26 07:38:53.000000 mosamaticdesktop-1.8.0/mosamaticdesktop/tasks/createpngfromtagfiletask/createpngfromtagfiletaskwidget.py
-drwxr-xr-x   0 Ralph      (501) staff       (20)        0 2024-01-26 14:35:23.956798 mosamaticdesktop-1.8.0/mosamaticdesktop/tasks/decompressdicomtask/
--rw-r--r--   0 Ralph      (501) staff       (20)        0 2024-01-26 07:38:53.000000 mosamaticdesktop-1.8.0/mosamaticdesktop/tasks/decompressdicomtask/__init__.py
--rw-r--r--   0 Ralph      (501) staff       (20)     2547 2024-01-26 14:29:31.000000 mosamaticdesktop-1.8.0/mosamaticdesktop/tasks/decompressdicomtask/decompressdicomtask.py
--rw-r--r--   0 Ralph      (501) staff       (20)     1206 2024-01-26 07:38:53.000000 mosamaticdesktop-1.8.0/mosamaticdesktop/tasks/decompressdicomtask/decompressdicomtaskwidget.py
--rw-r--r--   0 Ralph      (501) staff       (20)      885 2024-01-26 07:38:53.000000 mosamaticdesktop-1.8.0/mosamaticdesktop/tasks/descriptionparameter.py
-drwxr-xr-x   0 Ralph      (501) staff       (20)        0 2024-01-26 14:35:23.957758 mosamaticdesktop-1.8.0/mosamaticdesktop/tasks/dummytask/
--rw-r--r--   0 Ralph      (501) staff       (20)        0 2024-01-26 07:38:53.000000 mosamaticdesktop-1.8.0/mosamaticdesktop/tasks/dummytask/__init__.py
--rw-r--r--   0 Ralph      (501) staff       (20)     1544 2024-01-26 07:38:53.000000 mosamaticdesktop-1.8.0/mosamaticdesktop/tasks/dummytask/dummytask.py
--rw-r--r--   0 Ralph      (501) staff       (20)      914 2024-01-26 07:38:53.000000 mosamaticdesktop-1.8.0/mosamaticdesktop/tasks/dummytask/dummytaskwidget.py
--rw-r--r--   0 Ralph      (501) staff       (20)     1847 2024-01-26 07:38:53.000000 mosamaticdesktop-1.8.0/mosamaticdesktop/tasks/filesetparameter.py
--rw-r--r--   0 Ralph      (501) staff       (20)     1380 2024-01-26 07:38:53.000000 mosamaticdesktop-1.8.0/mosamaticdesktop/tasks/floatingpointparameter.py
--rw-r--r--   0 Ralph      (501) staff       (20)     1835 2024-01-26 07:38:53.000000 mosamaticdesktop-1.8.0/mosamaticdesktop/tasks/integerparameter.py
--rw-r--r--   0 Ralph      (501) staff       (20)     1154 2024-01-26 07:38:53.000000 mosamaticdesktop-1.8.0/mosamaticdesktop/tasks/labelparameter.py
--rw-r--r--   0 Ralph      (501) staff       (20)     2984 2024-01-26 07:38:53.000000 mosamaticdesktop-1.8.0/mosamaticdesktop/tasks/multifilesetparameter.py
-drwxr-xr-x   0 Ralph      (501) staff       (20)        0 2024-01-26 14:35:23.958554 mosamaticdesktop-1.8.0/mosamaticdesktop/tasks/musclefatsegmentationtask/
--rw-r--r--   0 Ralph      (501) staff       (20)        0 2024-01-26 07:38:53.000000 mosamaticdesktop-1.8.0/mosamaticdesktop/tasks/musclefatsegmentationtask/__init__.py
--rw-r--r--   0 Ralph      (501) staff       (20)     8820 2024-01-26 14:29:19.000000 mosamaticdesktop-1.8.0/mosamaticdesktop/tasks/musclefatsegmentationtask/musclefatsegmentationtask.py
--rw-r--r--   0 Ralph      (501) staff       (20)     1546 2024-01-26 07:38:53.000000 mosamaticdesktop-1.8.0/mosamaticdesktop/tasks/musclefatsegmentationtask/musclefatsegmentationtaskwidget.py
--rw-r--r--   0 Ralph      (501) staff       (20)     1658 2024-01-26 07:38:53.000000 mosamaticdesktop-1.8.0/mosamaticdesktop/tasks/optiongroupparameter.py
--rw-r--r--   0 Ralph      (501) staff       (20)     1427 2024-01-26 07:38:53.000000 mosamaticdesktop-1.8.0/mosamaticdesktop/tasks/parameter.py
--rw-r--r--   0 Ralph      (501) staff       (20)     1075 2024-01-26 07:38:53.000000 mosamaticdesktop-1.8.0/mosamaticdesktop/tasks/parametercopier.py
--rw-r--r--   0 Ralph      (501) staff       (20)     1528 2024-01-26 07:38:53.000000 mosamaticdesktop-1.8.0/mosamaticdesktop/tasks/pathparameter.py
--rw-r--r--   0 Ralph      (501) staff       (20)     5308 2024-01-26 07:38:53.000000 mosamaticdesktop-1.8.0/mosamaticdesktop/tasks/task.py
--rw-r--r--   0 Ralph      (501) staff       (20)     2043 2024-01-26 07:38:53.000000 mosamaticdesktop-1.8.0/mosamaticdesktop/tasks/taskruninfodialog.py
--rw-r--r--   0 Ralph      (501) staff       (20)    12757 2024-01-26 07:38:53.000000 mosamaticdesktop-1.8.0/mosamaticdesktop/tasks/taskwidget.py
--rw-r--r--   0 Ralph      (501) staff       (20)       46 2024-01-26 07:38:53.000000 mosamaticdesktop-1.8.0/mosamaticdesktop/tasks/taskwidgetexception.py
--rw-r--r--   0 Ralph      (501) staff       (20)     1545 2024-01-26 07:38:53.000000 mosamaticdesktop-1.8.0/mosamaticdesktop/tasks/taskwidgetmanager.py
--rw-r--r--   0 Ralph      (501) staff       (20)     2214 2024-01-26 07:38:53.000000 mosamaticdesktop-1.8.0/mosamaticdesktop/tasks/taskwidgetparameterdialog.py
--rw-r--r--   0 Ralph      (501) staff       (20)     1289 2024-01-26 07:38:53.000000 mosamaticdesktop-1.8.0/mosamaticdesktop/tasks/textparameter.py
--rw-r--r--   0 Ralph      (501) staff       (20)    13193 2024-01-26 11:34:09.000000 mosamaticdesktop-1.8.0/mosamaticdesktop/utils.py
-drwxr-xr-x   0 Ralph      (501) staff       (20)        0 2024-01-26 14:35:23.963229 mosamaticdesktop-1.8.0/mosamaticdesktop/widgets/
--rw-r--r--   0 Ralph      (501) staff       (20)        0 2024-01-26 07:38:53.000000 mosamaticdesktop-1.8.0/mosamaticdesktop/widgets/__init__.py
--rw-r--r--   0 Ralph      (501) staff       (20)      533 2024-01-26 07:38:53.000000 mosamaticdesktop-1.8.0/mosamaticdesktop/widgets/datadockwidget.py
--rw-r--r--   0 Ralph      (501) staff       (20)      844 2024-01-26 07:38:53.000000 mosamaticdesktop-1.8.0/mosamaticdesktop/widgets/dockwidget.py
--rw-r--r--   0 Ralph      (501) staff       (20)      511 2024-01-26 07:38:53.000000 mosamaticdesktop-1.8.0/mosamaticdesktop/widgets/fileitem.py
--rw-r--r--   0 Ralph      (501) staff       (20)      981 2024-01-26 07:38:53.000000 mosamaticdesktop-1.8.0/mosamaticdesktop/widgets/fileitemmenu.py
--rw-r--r--   0 Ralph      (501) staff       (20)      706 2024-01-26 07:38:53.000000 mosamaticdesktop-1.8.0/mosamaticdesktop/widgets/filesetitem.py
--rw-r--r--   0 Ralph      (501) staff       (20)     1175 2024-01-26 07:38:53.000000 mosamaticdesktop-1.8.0/mosamaticdesktop/widgets/filesetitemmenu.py
--rw-r--r--   0 Ralph      (501) staff       (20)     2892 2024-01-26 07:38:53.000000 mosamaticdesktop-1.8.0/mosamaticdesktop/widgets/filesettreeview.py
--rw-r--r--   0 Ralph      (501) staff       (20)      910 2024-01-26 07:38:53.000000 mosamaticdesktop-1.8.0/mosamaticdesktop/widgets/mainviewerdockwidget.py
--rw-r--r--   0 Ralph      (501) staff       (20)      226 2024-01-26 07:38:53.000000 mosamaticdesktop-1.8.0/mosamaticdesktop/widgets/progressbarwidget.py
--rw-r--r--   0 Ralph      (501) staff       (20)     1946 2024-01-26 07:38:53.000000 mosamaticdesktop-1.8.0/mosamaticdesktop/widgets/taskdockwidget.py
-drwxr-xr-x   0 Ralph      (501) staff       (20)        0 2024-01-26 14:35:23.963478 mosamaticdesktop-1.8.0/mosamaticdesktop/widgets/viewers/
--rw-r--r--   0 Ralph      (501) staff       (20)        0 2024-01-26 07:38:53.000000 mosamaticdesktop-1.8.0/mosamaticdesktop/widgets/viewers/__init__.py
-drwxr-xr-x   0 Ralph      (501) staff       (20)        0 2024-01-26 14:35:23.967162 mosamaticdesktop-1.8.0/mosamaticdesktop/widgets/viewers/dicomviewer/
--rw-r--r--   0 Ralph      (501) staff       (20)        0 2024-01-26 07:38:53.000000 mosamaticdesktop-1.8.0/mosamaticdesktop/widgets/viewers/dicomviewer/__init__.py
--rw-r--r--   0 Ralph      (501) staff       (20)     1115 2024-01-26 07:38:53.000000 mosamaticdesktop-1.8.0/mosamaticdesktop/widgets/viewers/dicomviewer/dicominfolayer.py
--rw-r--r--   0 Ralph      (501) staff       (20)     2220 2024-01-26 07:38:53.000000 mosamaticdesktop-1.8.0/mosamaticdesktop/widgets/viewers/dicomviewer/dicomlayer.py
--rw-r--r--   0 Ralph      (501) staff       (20)    11726 2024-01-26 13:25:59.000000 mosamaticdesktop-1.8.0/mosamaticdesktop/widgets/viewers/dicomviewer/dicomviewer.py
--rw-r--r--   0 Ralph      (501) staff       (20)      617 2024-01-26 07:38:53.000000 mosamaticdesktop-1.8.0/mosamaticdesktop/widgets/viewers/dicomviewer/filesetcombobox.py
--rw-r--r--   0 Ralph      (501) staff       (20)      111 2024-01-26 07:38:53.000000 mosamaticdesktop-1.8.0/mosamaticdesktop/widgets/viewers/dicomviewer/filesetloader.py
--rw-r--r--   0 Ralph      (501) staff       (20)     1059 2024-01-26 07:38:53.000000 mosamaticdesktop-1.8.0/mosamaticdesktop/widgets/viewers/dicomviewer/layer.py
--rw-r--r--   0 Ralph      (501) staff       (20)     1393 2024-01-26 07:38:53.000000 mosamaticdesktop-1.8.0/mosamaticdesktop/widgets/viewers/dicomviewer/segmentationlayer.py
--rw-r--r--   0 Ralph      (501) staff       (20)     1637 2024-01-26 07:38:53.000000 mosamaticdesktop-1.8.0/mosamaticdesktop/widgets/viewers/dicomviewer/taglayer.py
-drwxr-xr-x   0 Ralph      (501) staff       (20)        0 2024-01-26 14:35:23.935518 mosamaticdesktop-1.8.0/mosamaticdesktop.egg-info/
--rw-r--r--   0 Ralph      (501) staff       (20)      690 2024-01-26 14:35:23.000000 mosamaticdesktop-1.8.0/mosamaticdesktop.egg-info/PKG-INFO
--rw-r--r--   0 Ralph      (501) staff       (20)     5136 2024-01-26 14:35:23.000000 mosamaticdesktop-1.8.0/mosamaticdesktop.egg-info/SOURCES.txt
--rw-r--r--   0 Ralph      (501) staff       (20)        1 2024-01-26 14:35:23.000000 mosamaticdesktop-1.8.0/mosamaticdesktop.egg-info/dependency_links.txt
--rw-r--r--   0 Ralph      (501) staff       (20)       65 2024-01-26 14:35:23.000000 mosamaticdesktop-1.8.0/mosamaticdesktop.egg-info/entry_points.txt
--rw-r--r--   0 Ralph      (501) staff       (20)        1 2024-01-26 10:53:29.000000 mosamaticdesktop-1.8.0/mosamaticdesktop.egg-info/not-zip-safe
--rw-r--r--   0 Ralph      (501) staff       (20)      149 2024-01-26 14:35:23.000000 mosamaticdesktop-1.8.0/mosamaticdesktop.egg-info/requires.txt
--rw-r--r--   0 Ralph      (501) staff       (20)       17 2024-01-26 14:35:23.000000 mosamaticdesktop-1.8.0/mosamaticdesktop.egg-info/top_level.txt
--rw-r--r--   0 Ralph      (501) staff       (20)       38 2024-01-26 14:35:23.968011 mosamaticdesktop-1.8.0/setup.cfg
--rw-r--r--   0 Ralph      (501) staff       (20)     1877 2024-01-26 11:09:01.000000 mosamaticdesktop-1.8.0/setup.py
+drwxr-xr-x   0 ralph      (501) staff       (20)        0 2024-01-26 17:32:57.913987 mosamaticdesktop-1.9.0/
+-rw-r--r--   0 ralph      (501) staff       (20)     1111 2024-01-26 17:32:57.913775 mosamaticdesktop-1.9.0/PKG-INFO
+drwxr-xr-x   0 ralph      (501) staff       (20)        0 2024-01-26 17:32:57.893652 mosamaticdesktop-1.9.0/mosamaticdesktop/
+-rw-r--r--   0 ralph      (501) staff       (20)        0 2024-01-23 17:59:08.000000 mosamaticdesktop-1.9.0/mosamaticdesktop/__init__.py
+drwxr-xr-x   0 ralph      (501) staff       (20)        0 2024-01-26 17:32:57.895480 mosamaticdesktop-1.9.0/mosamaticdesktop/ai/
+-rw-r--r--   0 ralph      (501) staff       (20)        0 2024-01-12 17:01:52.000000 mosamaticdesktop-1.9.0/mosamaticdesktop/ai/__init__.py
+-rw-r--r--   0 ralph      (501) staff       (20)      266 2024-01-12 17:01:52.000000 mosamaticdesktop-1.9.0/mosamaticdesktop/ai/model.py
+-rw-r--r--   0 ralph      (501) staff       (20)      432 2024-01-25 15:12:09.000000 mosamaticdesktop-1.9.0/mosamaticdesktop/ai/pytorchmodel.py
+-rw-r--r--   0 ralph      (501) staff       (20)      536 2024-01-25 15:12:09.000000 mosamaticdesktop-1.9.0/mosamaticdesktop/ai/tensorflowmodel.py
+drwxr-xr-x   0 ralph      (501) staff       (20)        0 2024-01-26 17:32:57.896770 mosamaticdesktop-1.9.0/mosamaticdesktop/data/
+-rw-r--r--   0 ralph      (501) staff       (20)        0 2024-01-05 18:01:37.000000 mosamaticdesktop-1.9.0/mosamaticdesktop/data/__init__.py
+-rw-r--r--   0 ralph      (501) staff       (20)     4446 2024-01-25 15:12:09.000000 mosamaticdesktop-1.9.0/mosamaticdesktop/data/datamanager.py
+-rw-r--r--   0 ralph      (501) staff       (20)      519 2024-01-25 15:12:09.000000 mosamaticdesktop-1.9.0/mosamaticdesktop/data/engine.py
+-rw-r--r--   0 ralph      (501) staff       (20)      374 2024-01-25 15:24:43.000000 mosamaticdesktop-1.9.0/mosamaticdesktop/data/file.py
+-rw-r--r--   0 ralph      (501) staff       (20)      395 2024-01-25 15:12:09.000000 mosamaticdesktop-1.9.0/mosamaticdesktop/data/filecontent.py
+-rw-r--r--   0 ralph      (501) staff       (20)      683 2024-01-25 15:12:09.000000 mosamaticdesktop-1.9.0/mosamaticdesktop/data/filecontentcache.py
+-rw-r--r--   0 ralph      (501) staff       (20)      894 2024-01-25 15:12:09.000000 mosamaticdesktop-1.9.0/mosamaticdesktop/data/fileset.py
+drwxr-xr-x   0 ralph      (501) staff       (20)        0 2024-01-26 17:32:57.897323 mosamaticdesktop-1.9.0/mosamaticdesktop/data/models/
+-rw-r--r--   0 ralph      (501) staff       (20)        0 2024-01-25 15:22:30.000000 mosamaticdesktop-1.9.0/mosamaticdesktop/data/models/__init__.py
+-rw-r--r--   0 ralph      (501) staff       (20)       87 2024-01-05 18:01:37.000000 mosamaticdesktop-1.9.0/mosamaticdesktop/data/models/basemodel.py
+-rw-r--r--   0 ralph      (501) staff       (20)      715 2024-01-25 15:12:09.000000 mosamaticdesktop-1.9.0/mosamaticdesktop/data/models/filemodel.py
+-rw-r--r--   0 ralph      (501) staff       (20)      724 2024-01-25 15:12:09.000000 mosamaticdesktop-1.9.0/mosamaticdesktop/data/models/filesetmodel.py
+-rw-r--r--   0 ralph      (501) staff       (20)      370 2024-01-25 15:12:09.000000 mosamaticdesktop-1.9.0/mosamaticdesktop/data/session.py
+-rw-r--r--   0 ralph      (501) staff       (20)     2216 2024-01-25 15:12:08.000000 mosamaticdesktop-1.9.0/mosamaticdesktop/logger.py
+-rw-r--r--   0 ralph      (501) staff       (20)      300 2024-01-25 15:03:44.000000 mosamaticdesktop-1.9.0/mosamaticdesktop/main.py
+-rw-r--r--   0 ralph      (501) staff       (20)      266 2024-01-25 15:12:08.000000 mosamaticdesktop-1.9.0/mosamaticdesktop/maintest.py
+-rw-r--r--   0 ralph      (501) staff       (20)     5711 2024-01-25 15:12:08.000000 mosamaticdesktop-1.9.0/mosamaticdesktop/mainwindow.py
+-rw-r--r--   0 ralph      (501) staff       (20)      475 2024-01-18 08:31:07.000000 mosamaticdesktop-1.9.0/mosamaticdesktop/operatingsystem.py
+drwxr-xr-x   0 ralph      (501) staff       (20)        0 2024-01-26 17:32:57.897699 mosamaticdesktop-1.9.0/mosamaticdesktop/scripts/
+-rw-r--r--   0 ralph      (501) staff       (20)      220 2024-01-26 16:06:14.000000 mosamaticdesktop-1.9.0/mosamaticdesktop/scripts/mosamatic.bat
+-rwxr-xr-x   0 ralph      (501) staff       (20)      135 2024-01-26 16:06:14.000000 mosamaticdesktop-1.9.0/mosamaticdesktop/scripts/mosamatic.sh
+-rw-r--r--   0 ralph      (501) staff       (20)      223 2024-01-05 18:01:37.000000 mosamaticdesktop-1.9.0/mosamaticdesktop/singleton.py
+drwxr-xr-x   0 ralph      (501) staff       (20)        0 2024-01-26 17:32:57.902181 mosamaticdesktop-1.9.0/mosamaticdesktop/tasks/
+-rw-r--r--   0 ralph      (501) staff       (20)        0 2024-01-06 19:07:35.000000 mosamaticdesktop-1.9.0/mosamaticdesktop/tasks/__init__.py
+-rw-r--r--   0 ralph      (501) staff       (20)     1454 2024-01-25 15:12:09.000000 mosamaticdesktop-1.9.0/mosamaticdesktop/tasks/booleanparameter.py
+drwxr-xr-x   0 ralph      (501) staff       (20)        0 2024-01-26 17:32:57.902627 mosamaticdesktop-1.9.0/mosamaticdesktop/tasks/calculatebodycompositionmetricstask/
+-rw-r--r--   0 ralph      (501) staff       (20)        0 2024-01-09 20:57:00.000000 mosamaticdesktop-1.9.0/mosamaticdesktop/tasks/calculatebodycompositionmetricstask/__init__.py
+-rw-r--r--   0 ralph      (501) staff       (20)    11453 2024-01-26 16:06:14.000000 mosamaticdesktop-1.9.0/mosamaticdesktop/tasks/calculatebodycompositionmetricstask/calculatebodycompositionmetricstask.py
+-rw-r--r--   0 ralph      (501) staff       (20)     1682 2024-01-25 15:12:09.000000 mosamaticdesktop-1.9.0/mosamaticdesktop/tasks/calculatebodycompositionmetricstask/calculatebodycompositionmetricstaskwidget.py
+drwxr-xr-x   0 ralph      (501) staff       (20)        0 2024-01-26 17:32:57.902992 mosamaticdesktop-1.9.0/mosamaticdesktop/tasks/checkdicomheadertask/
+-rw-r--r--   0 ralph      (501) staff       (20)        0 2024-01-25 15:38:58.000000 mosamaticdesktop-1.9.0/mosamaticdesktop/tasks/checkdicomheadertask/__init__.py
+-rw-r--r--   0 ralph      (501) staff       (20)     3566 2024-01-26 16:06:14.000000 mosamaticdesktop-1.9.0/mosamaticdesktop/tasks/checkdicomheadertask/checkdicomheadertask.py
+-rw-r--r--   0 ralph      (501) staff       (20)     2345 2024-01-25 15:12:09.000000 mosamaticdesktop-1.9.0/mosamaticdesktop/tasks/checkdicomheadertask/checkdicomheadertaskwidget.py
+drwxr-xr-x   0 ralph      (501) staff       (20)        0 2024-01-26 17:32:57.903359 mosamaticdesktop-1.9.0/mosamaticdesktop/tasks/copyfilesettask/
+-rw-r--r--   0 ralph      (501) staff       (20)        0 2024-01-13 16:23:38.000000 mosamaticdesktop-1.9.0/mosamaticdesktop/tasks/copyfilesettask/__init__.py
+-rw-r--r--   0 ralph      (501) staff       (20)     1919 2024-01-26 16:06:14.000000 mosamaticdesktop-1.9.0/mosamaticdesktop/tasks/copyfilesettask/copyfilesettask.py
+-rw-r--r--   0 ralph      (501) staff       (20)     1170 2024-01-25 15:12:09.000000 mosamaticdesktop-1.9.0/mosamaticdesktop/tasks/copyfilesettask/copyfilesettaskwidget.py
+drwxr-xr-x   0 ralph      (501) staff       (20)        0 2024-01-26 17:32:57.903734 mosamaticdesktop-1.9.0/mosamaticdesktop/tasks/createarchivetask/
+-rw-r--r--   0 ralph      (501) staff       (20)        0 2024-01-13 17:54:18.000000 mosamaticdesktop-1.9.0/mosamaticdesktop/tasks/createarchivetask/__init__.py
+-rw-r--r--   0 ralph      (501) staff       (20)     1803 2024-01-26 16:06:14.000000 mosamaticdesktop-1.9.0/mosamaticdesktop/tasks/createarchivetask/createarchivetask.py
+-rw-r--r--   0 ralph      (501) staff       (20)     1157 2024-01-25 15:12:09.000000 mosamaticdesktop-1.9.0/mosamaticdesktop/tasks/createarchivetask/createarchivetaskwidget.py
+drwxr-xr-x   0 ralph      (501) staff       (20)        0 2024-01-26 17:32:57.904069 mosamaticdesktop-1.9.0/mosamaticdesktop/tasks/createpngfromdicomfiletask/
+-rw-r--r--   0 ralph      (501) staff       (20)        0 2024-01-25 15:39:09.000000 mosamaticdesktop-1.9.0/mosamaticdesktop/tasks/createpngfromdicomfiletask/__init__.py
+-rw-r--r--   0 ralph      (501) staff       (20)     2562 2024-01-26 16:06:14.000000 mosamaticdesktop-1.9.0/mosamaticdesktop/tasks/createpngfromdicomfiletask/createpngfromdicomfiletask.py
+-rw-r--r--   0 ralph      (501) staff       (20)     1633 2024-01-25 15:12:09.000000 mosamaticdesktop-1.9.0/mosamaticdesktop/tasks/createpngfromdicomfiletask/createpngfromdicomfiletaskwidget.py
+drwxr-xr-x   0 ralph      (501) staff       (20)        0 2024-01-26 17:32:57.904547 mosamaticdesktop-1.9.0/mosamaticdesktop/tasks/createpngfromsegmentationfiletask/
+-rw-r--r--   0 ralph      (501) staff       (20)        0 2024-01-26 16:06:14.000000 mosamaticdesktop-1.9.0/mosamaticdesktop/tasks/createpngfromsegmentationfiletask/__init__.py
+-rw-r--r--   0 ralph      (501) staff       (20)     2369 2024-01-26 16:06:14.000000 mosamaticdesktop-1.9.0/mosamaticdesktop/tasks/createpngfromsegmentationfiletask/createpngfromsegmentationfiletask.py
+-rw-r--r--   0 ralph      (501) staff       (20)     1236 2024-01-26 16:06:14.000000 mosamaticdesktop-1.9.0/mosamaticdesktop/tasks/createpngfromsegmentationfiletask/createpngfromsegmentationfiletaskwidget.py
+drwxr-xr-x   0 ralph      (501) staff       (20)        0 2024-01-26 17:32:57.905218 mosamaticdesktop-1.9.0/mosamaticdesktop/tasks/createpngfromtagfiletask/
+-rw-r--r--   0 ralph      (501) staff       (20)        0 2024-01-25 15:39:17.000000 mosamaticdesktop-1.9.0/mosamaticdesktop/tasks/createpngfromtagfiletask/__init__.py
+-rw-r--r--   0 ralph      (501) staff       (20)     2312 2024-01-26 16:06:14.000000 mosamaticdesktop-1.9.0/mosamaticdesktop/tasks/createpngfromtagfiletask/createpngfromtagfiletask.py
+-rw-r--r--   0 ralph      (501) staff       (20)     1194 2024-01-25 15:12:09.000000 mosamaticdesktop-1.9.0/mosamaticdesktop/tasks/createpngfromtagfiletask/createpngfromtagfiletaskwidget.py
+drwxr-xr-x   0 ralph      (501) staff       (20)        0 2024-01-26 17:32:57.905715 mosamaticdesktop-1.9.0/mosamaticdesktop/tasks/decompressdicomtask/
+-rw-r--r--   0 ralph      (501) staff       (20)        0 2024-01-25 15:39:20.000000 mosamaticdesktop-1.9.0/mosamaticdesktop/tasks/decompressdicomtask/__init__.py
+-rw-r--r--   0 ralph      (501) staff       (20)     2547 2024-01-26 16:06:14.000000 mosamaticdesktop-1.9.0/mosamaticdesktop/tasks/decompressdicomtask/decompressdicomtask.py
+-rw-r--r--   0 ralph      (501) staff       (20)     1206 2024-01-25 15:12:09.000000 mosamaticdesktop-1.9.0/mosamaticdesktop/tasks/decompressdicomtask/decompressdicomtaskwidget.py
+-rw-r--r--   0 ralph      (501) staff       (20)      885 2024-01-25 15:12:09.000000 mosamaticdesktop-1.9.0/mosamaticdesktop/tasks/descriptionparameter.py
+drwxr-xr-x   0 ralph      (501) staff       (20)        0 2024-01-26 17:32:57.906122 mosamaticdesktop-1.9.0/mosamaticdesktop/tasks/dummytask/
+-rw-r--r--   0 ralph      (501) staff       (20)        0 2024-01-05 18:01:37.000000 mosamaticdesktop-1.9.0/mosamaticdesktop/tasks/dummytask/__init__.py
+-rw-r--r--   0 ralph      (501) staff       (20)     1544 2024-01-25 15:12:09.000000 mosamaticdesktop-1.9.0/mosamaticdesktop/tasks/dummytask/dummytask.py
+-rw-r--r--   0 ralph      (501) staff       (20)      914 2024-01-25 15:12:09.000000 mosamaticdesktop-1.9.0/mosamaticdesktop/tasks/dummytask/dummytaskwidget.py
+-rw-r--r--   0 ralph      (501) staff       (20)     1847 2024-01-25 15:12:09.000000 mosamaticdesktop-1.9.0/mosamaticdesktop/tasks/filesetparameter.py
+-rw-r--r--   0 ralph      (501) staff       (20)     1380 2024-01-25 15:12:09.000000 mosamaticdesktop-1.9.0/mosamaticdesktop/tasks/floatingpointparameter.py
+-rw-r--r--   0 ralph      (501) staff       (20)     1835 2024-01-25 15:12:09.000000 mosamaticdesktop-1.9.0/mosamaticdesktop/tasks/integerparameter.py
+-rw-r--r--   0 ralph      (501) staff       (20)     1154 2024-01-25 15:12:09.000000 mosamaticdesktop-1.9.0/mosamaticdesktop/tasks/labelparameter.py
+-rw-r--r--   0 ralph      (501) staff       (20)     2984 2024-01-25 15:12:09.000000 mosamaticdesktop-1.9.0/mosamaticdesktop/tasks/multifilesetparameter.py
+drwxr-xr-x   0 ralph      (501) staff       (20)        0 2024-01-26 17:32:57.906642 mosamaticdesktop-1.9.0/mosamaticdesktop/tasks/musclefatsegmentationtask/
+-rw-r--r--   0 ralph      (501) staff       (20)        0 2024-01-09 17:48:27.000000 mosamaticdesktop-1.9.0/mosamaticdesktop/tasks/musclefatsegmentationtask/__init__.py
+-rw-r--r--   0 ralph      (501) staff       (20)     8820 2024-01-26 16:06:14.000000 mosamaticdesktop-1.9.0/mosamaticdesktop/tasks/musclefatsegmentationtask/musclefatsegmentationtask.py
+-rw-r--r--   0 ralph      (501) staff       (20)     1546 2024-01-25 15:12:09.000000 mosamaticdesktop-1.9.0/mosamaticdesktop/tasks/musclefatsegmentationtask/musclefatsegmentationtaskwidget.py
+-rw-r--r--   0 ralph      (501) staff       (20)     1658 2024-01-25 15:12:09.000000 mosamaticdesktop-1.9.0/mosamaticdesktop/tasks/optiongroupparameter.py
+-rw-r--r--   0 ralph      (501) staff       (20)     1427 2024-01-09 16:31:30.000000 mosamaticdesktop-1.9.0/mosamaticdesktop/tasks/parameter.py
+-rw-r--r--   0 ralph      (501) staff       (20)     1075 2024-01-25 15:12:09.000000 mosamaticdesktop-1.9.0/mosamaticdesktop/tasks/parametercopier.py
+-rw-r--r--   0 ralph      (501) staff       (20)     1528 2024-01-25 15:12:09.000000 mosamaticdesktop-1.9.0/mosamaticdesktop/tasks/pathparameter.py
+-rw-r--r--   0 ralph      (501) staff       (20)     5308 2024-01-25 15:12:09.000000 mosamaticdesktop-1.9.0/mosamaticdesktop/tasks/task.py
+-rw-r--r--   0 ralph      (501) staff       (20)     2043 2024-01-09 16:31:30.000000 mosamaticdesktop-1.9.0/mosamaticdesktop/tasks/taskruninfodialog.py
+-rw-r--r--   0 ralph      (501) staff       (20)    12757 2024-01-25 15:12:09.000000 mosamaticdesktop-1.9.0/mosamaticdesktop/tasks/taskwidget.py
+-rw-r--r--   0 ralph      (501) staff       (20)       46 2024-01-06 07:12:34.000000 mosamaticdesktop-1.9.0/mosamaticdesktop/tasks/taskwidgetexception.py
+-rw-r--r--   0 ralph      (501) staff       (20)     1545 2024-01-25 15:12:09.000000 mosamaticdesktop-1.9.0/mosamaticdesktop/tasks/taskwidgetmanager.py
+-rw-r--r--   0 ralph      (501) staff       (20)     2214 2024-01-25 15:12:09.000000 mosamaticdesktop-1.9.0/mosamaticdesktop/tasks/taskwidgetparameterdialog.py
+-rw-r--r--   0 ralph      (501) staff       (20)     1289 2024-01-25 15:12:09.000000 mosamaticdesktop-1.9.0/mosamaticdesktop/tasks/textparameter.py
+drwxr-xr-x   0 ralph      (501) staff       (20)        0 2024-01-26 17:32:57.907211 mosamaticdesktop-1.9.0/mosamaticdesktop/tasks/totalsegmentatorroiselectiontask/
+-rw-r--r--   0 ralph      (501) staff       (20)        0 2024-01-26 17:03:39.000000 mosamaticdesktop-1.9.0/mosamaticdesktop/tasks/totalsegmentatorroiselectiontask/__init__.py
+-rw-r--r--   0 ralph      (501) staff       (20)     3094 2024-01-26 17:31:14.000000 mosamaticdesktop-1.9.0/mosamaticdesktop/tasks/totalsegmentatorroiselectiontask/totalsegmentatorroiselectiontask.py
+-rw-r--r--   0 ralph      (501) staff       (20)     4469 2024-01-26 17:22:05.000000 mosamaticdesktop-1.9.0/mosamaticdesktop/tasks/totalsegmentatorroiselectiontask/totalsegmentatorroiselectiontaskwidget.py
+drwxr-xr-x   0 ralph      (501) staff       (20)        0 2024-01-26 17:32:57.907748 mosamaticdesktop-1.9.0/mosamaticdesktop/tasks/totalsegmentatortask/
+-rw-r--r--   0 ralph      (501) staff       (20)        0 2024-01-26 16:06:14.000000 mosamaticdesktop-1.9.0/mosamaticdesktop/tasks/totalsegmentatortask/__init__.py
+-rw-r--r--   0 ralph      (501) staff       (20)     2947 2024-01-26 17:02:51.000000 mosamaticdesktop-1.9.0/mosamaticdesktop/tasks/totalsegmentatortask/totalsegmentatortask.py
+-rw-r--r--   0 ralph      (501) staff       (20)     1262 2024-01-26 16:06:14.000000 mosamaticdesktop-1.9.0/mosamaticdesktop/tasks/totalsegmentatortask/totalsegmentatortaskwidget.py
+-rw-r--r--   0 ralph      (501) staff       (20)    13193 2024-01-26 16:06:14.000000 mosamaticdesktop-1.9.0/mosamaticdesktop/utils.py
+drwxr-xr-x   0 ralph      (501) staff       (20)        0 2024-01-26 17:32:57.911949 mosamaticdesktop-1.9.0/mosamaticdesktop/widgets/
+-rw-r--r--   0 ralph      (501) staff       (20)        0 2024-01-25 15:27:07.000000 mosamaticdesktop-1.9.0/mosamaticdesktop/widgets/__init__.py
+-rw-r--r--   0 ralph      (501) staff       (20)      533 2024-01-25 15:12:09.000000 mosamaticdesktop-1.9.0/mosamaticdesktop/widgets/datadockwidget.py
+-rw-r--r--   0 ralph      (501) staff       (20)      844 2024-01-05 18:45:08.000000 mosamaticdesktop-1.9.0/mosamaticdesktop/widgets/dockwidget.py
+-rw-r--r--   0 ralph      (501) staff       (20)      511 2024-01-25 15:12:09.000000 mosamaticdesktop-1.9.0/mosamaticdesktop/widgets/fileitem.py
+-rw-r--r--   0 ralph      (501) staff       (20)      981 2024-01-25 15:12:09.000000 mosamaticdesktop-1.9.0/mosamaticdesktop/widgets/fileitemmenu.py
+-rw-r--r--   0 ralph      (501) staff       (20)      706 2024-01-25 15:12:09.000000 mosamaticdesktop-1.9.0/mosamaticdesktop/widgets/filesetitem.py
+-rw-r--r--   0 ralph      (501) staff       (20)     1175 2024-01-25 15:12:09.000000 mosamaticdesktop-1.9.0/mosamaticdesktop/widgets/filesetitemmenu.py
+-rw-r--r--   0 ralph      (501) staff       (20)     2892 2024-01-25 15:12:09.000000 mosamaticdesktop-1.9.0/mosamaticdesktop/widgets/filesettreeview.py
+-rw-r--r--   0 ralph      (501) staff       (20)      910 2024-01-25 15:12:09.000000 mosamaticdesktop-1.9.0/mosamaticdesktop/widgets/mainviewerdockwidget.py
+-rw-r--r--   0 ralph      (501) staff       (20)      226 2024-01-25 15:12:09.000000 mosamaticdesktop-1.9.0/mosamaticdesktop/widgets/progressbarwidget.py
+-rw-r--r--   0 ralph      (501) staff       (20)     1946 2024-01-25 15:12:08.000000 mosamaticdesktop-1.9.0/mosamaticdesktop/widgets/taskdockwidget.py
+drwxr-xr-x   0 ralph      (501) staff       (20)        0 2024-01-26 17:32:57.912183 mosamaticdesktop-1.9.0/mosamaticdesktop/widgets/viewers/
+-rw-r--r--   0 ralph      (501) staff       (20)        0 2024-01-15 15:09:23.000000 mosamaticdesktop-1.9.0/mosamaticdesktop/widgets/viewers/__init__.py
+drwxr-xr-x   0 ralph      (501) staff       (20)        0 2024-01-26 17:32:57.913476 mosamaticdesktop-1.9.0/mosamaticdesktop/widgets/viewers/dicomviewer/
+-rw-r--r--   0 ralph      (501) staff       (20)        0 2024-01-15 15:09:33.000000 mosamaticdesktop-1.9.0/mosamaticdesktop/widgets/viewers/dicomviewer/__init__.py
+-rw-r--r--   0 ralph      (501) staff       (20)     1115 2024-01-25 15:12:09.000000 mosamaticdesktop-1.9.0/mosamaticdesktop/widgets/viewers/dicomviewer/dicominfolayer.py
+-rw-r--r--   0 ralph      (501) staff       (20)     2220 2024-01-25 15:12:09.000000 mosamaticdesktop-1.9.0/mosamaticdesktop/widgets/viewers/dicomviewer/dicomlayer.py
+-rw-r--r--   0 ralph      (501) staff       (20)    11726 2024-01-26 16:06:14.000000 mosamaticdesktop-1.9.0/mosamaticdesktop/widgets/viewers/dicomviewer/dicomviewer.py
+-rw-r--r--   0 ralph      (501) staff       (20)      617 2024-01-25 15:12:09.000000 mosamaticdesktop-1.9.0/mosamaticdesktop/widgets/viewers/dicomviewer/filesetcombobox.py
+-rw-r--r--   0 ralph      (501) staff       (20)      111 2024-01-23 17:16:08.000000 mosamaticdesktop-1.9.0/mosamaticdesktop/widgets/viewers/dicomviewer/filesetloader.py
+-rw-r--r--   0 ralph      (501) staff       (20)     1059 2024-01-25 15:12:09.000000 mosamaticdesktop-1.9.0/mosamaticdesktop/widgets/viewers/dicomviewer/layer.py
+-rw-r--r--   0 ralph      (501) staff       (20)     1393 2024-01-25 15:12:09.000000 mosamaticdesktop-1.9.0/mosamaticdesktop/widgets/viewers/dicomviewer/segmentationlayer.py
+-rw-r--r--   0 ralph      (501) staff       (20)     1637 2024-01-25 15:12:09.000000 mosamaticdesktop-1.9.0/mosamaticdesktop/widgets/viewers/dicomviewer/taglayer.py
+drwxr-xr-x   0 ralph      (501) staff       (20)        0 2024-01-26 17:32:57.894729 mosamaticdesktop-1.9.0/mosamaticdesktop.egg-info/
+-rw-r--r--   0 ralph      (501) staff       (20)     1111 2024-01-26 17:32:57.000000 mosamaticdesktop-1.9.0/mosamaticdesktop.egg-info/PKG-INFO
+-rw-r--r--   0 ralph      (501) staff       (20)     5592 2024-01-26 17:32:57.000000 mosamaticdesktop-1.9.0/mosamaticdesktop.egg-info/SOURCES.txt
+-rw-r--r--   0 ralph      (501) staff       (20)        1 2024-01-26 17:32:57.000000 mosamaticdesktop-1.9.0/mosamaticdesktop.egg-info/dependency_links.txt
+-rw-r--r--   0 ralph      (501) staff       (20)       65 2024-01-26 17:32:57.000000 mosamaticdesktop-1.9.0/mosamaticdesktop.egg-info/entry_points.txt
+-rw-r--r--   0 ralph      (501) staff       (20)        1 2024-01-25 15:02:06.000000 mosamaticdesktop-1.9.0/mosamaticdesktop.egg-info/not-zip-safe
+-rw-r--r--   0 ralph      (501) staff       (20)      166 2024-01-26 17:32:57.000000 mosamaticdesktop-1.9.0/mosamaticdesktop.egg-info/requires.txt
+-rw-r--r--   0 ralph      (501) staff       (20)       17 2024-01-26 17:32:57.000000 mosamaticdesktop-1.9.0/mosamaticdesktop.egg-info/top_level.txt
+-rw-r--r--   0 ralph      (501) staff       (20)       38 2024-01-26 17:32:57.914020 mosamaticdesktop-1.9.0/setup.cfg
+-rw-r--r--   0 ralph      (501) staff       (20)     1877 2024-01-26 16:06:14.000000 mosamaticdesktop-1.9.0/setup.py
```

### Comparing `mosamaticdesktop-1.8.0/mosamaticdesktop/ai/tensorflowmodel.py` & `mosamaticdesktop-1.9.0/mosamaticdesktop/ai/tensorflowmodel.py`

 * *Files identical despite different names*

### Comparing `mosamaticdesktop-1.8.0/mosamaticdesktop/data/datamanager.py` & `mosamaticdesktop-1.9.0/mosamaticdesktop/data/datamanager.py`

 * *Files identical despite different names*

### Comparing `mosamaticdesktop-1.8.0/mosamaticdesktop/data/engine.py` & `mosamaticdesktop-1.9.0/mosamaticdesktop/data/engine.py`

 * *Files identical despite different names*

### Comparing `mosamaticdesktop-1.8.0/mosamaticdesktop/data/filecontentcache.py` & `mosamaticdesktop-1.9.0/mosamaticdesktop/data/filecontentcache.py`

 * *Files identical despite different names*

### Comparing `mosamaticdesktop-1.8.0/mosamaticdesktop/data/fileset.py` & `mosamaticdesktop-1.9.0/mosamaticdesktop/data/fileset.py`

 * *Files identical despite different names*

### Comparing `mosamaticdesktop-1.8.0/mosamaticdesktop/data/models/filemodel.py` & `mosamaticdesktop-1.9.0/mosamaticdesktop/data/models/filemodel.py`

 * *Files identical despite different names*

### Comparing `mosamaticdesktop-1.8.0/mosamaticdesktop/data/models/filesetmodel.py` & `mosamaticdesktop-1.9.0/mosamaticdesktop/data/models/filesetmodel.py`

 * *Files identical despite different names*

### Comparing `mosamaticdesktop-1.8.0/mosamaticdesktop/logger.py` & `mosamaticdesktop-1.9.0/mosamaticdesktop/logger.py`

 * *Files identical despite different names*

### Comparing `mosamaticdesktop-1.8.0/mosamaticdesktop/mainwindow.py` & `mosamaticdesktop-1.9.0/mosamaticdesktop/mainwindow.py`

 * *Files identical despite different names*

### Comparing `mosamaticdesktop-1.8.0/mosamaticdesktop/tasks/booleanparameter.py` & `mosamaticdesktop-1.9.0/mosamaticdesktop/tasks/booleanparameter.py`

 * *Files identical despite different names*

### Comparing `mosamaticdesktop-1.8.0/mosamaticdesktop/tasks/calculatebodycompositionmetricstask/calculatebodycompositionmetricstask.py` & `mosamaticdesktop-1.9.0/mosamaticdesktop/tasks/calculatebodycompositionmetricstask/calculatebodycompositionmetricstask.py`

 * *Files identical despite different names*

### Comparing `mosamaticdesktop-1.8.0/mosamaticdesktop/tasks/calculatebodycompositionmetricstask/calculatebodycompositionmetricstaskwidget.py` & `mosamaticdesktop-1.9.0/mosamaticdesktop/tasks/calculatebodycompositionmetricstask/calculatebodycompositionmetricstaskwidget.py`

 * *Files identical despite different names*

### Comparing `mosamaticdesktop-1.8.0/mosamaticdesktop/tasks/checkdicomheadertask/checkdicomheadertask.py` & `mosamaticdesktop-1.9.0/mosamaticdesktop/tasks/checkdicomheadertask/checkdicomheadertask.py`

 * *Files identical despite different names*

### Comparing `mosamaticdesktop-1.8.0/mosamaticdesktop/tasks/checkdicomheadertask/checkdicomheadertaskwidget.py` & `mosamaticdesktop-1.9.0/mosamaticdesktop/tasks/checkdicomheadertask/checkdicomheadertaskwidget.py`

 * *Files identical despite different names*

### Comparing `mosamaticdesktop-1.8.0/mosamaticdesktop/tasks/copyfilesettask/copyfilesettask.py` & `mosamaticdesktop-1.9.0/mosamaticdesktop/tasks/copyfilesettask/copyfilesettask.py`

 * *Files identical despite different names*

### Comparing `mosamaticdesktop-1.8.0/mosamaticdesktop/tasks/copyfilesettask/copyfilesettaskwidget.py` & `mosamaticdesktop-1.9.0/mosamaticdesktop/tasks/copyfilesettask/copyfilesettaskwidget.py`

 * *Files identical despite different names*

### Comparing `mosamaticdesktop-1.8.0/mosamaticdesktop/tasks/createarchivetask/createarchivetask.py` & `mosamaticdesktop-1.9.0/mosamaticdesktop/tasks/createarchivetask/createarchivetask.py`

 * *Files identical despite different names*

### Comparing `mosamaticdesktop-1.8.0/mosamaticdesktop/tasks/createarchivetask/createarchivetaskwidget.py` & `mosamaticdesktop-1.9.0/mosamaticdesktop/tasks/createarchivetask/createarchivetaskwidget.py`

 * *Files identical despite different names*

### Comparing `mosamaticdesktop-1.8.0/mosamaticdesktop/tasks/createpngfromdicomfiletask/createpngfromdicomfiletask.py` & `mosamaticdesktop-1.9.0/mosamaticdesktop/tasks/createpngfromdicomfiletask/createpngfromdicomfiletask.py`

 * *Files identical despite different names*

### Comparing `mosamaticdesktop-1.8.0/mosamaticdesktop/tasks/createpngfromdicomfiletask/createpngfromdicomfiletaskwidget.py` & `mosamaticdesktop-1.9.0/mosamaticdesktop/tasks/createpngfromdicomfiletask/createpngfromdicomfiletaskwidget.py`

 * *Files identical despite different names*

### Comparing `mosamaticdesktop-1.8.0/mosamaticdesktop/tasks/createpngfromsegmentationfiletask/createpngfromsegmentationfiletask.py` & `mosamaticdesktop-1.9.0/mosamaticdesktop/tasks/createpngfromsegmentationfiletask/createpngfromsegmentationfiletask.py`

 * *Files identical despite different names*

### Comparing `mosamaticdesktop-1.8.0/mosamaticdesktop/tasks/createpngfromsegmentationfiletask/createpngfromsegmentationfiletaskwidget.py` & `mosamaticdesktop-1.9.0/mosamaticdesktop/tasks/createpngfromsegmentationfiletask/createpngfromsegmentationfiletaskwidget.py`

 * *Files identical despite different names*

### Comparing `mosamaticdesktop-1.8.0/mosamaticdesktop/tasks/createpngfromtagfiletask/createpngfromtagfiletask.py` & `mosamaticdesktop-1.9.0/mosamaticdesktop/tasks/createpngfromtagfiletask/createpngfromtagfiletask.py`

 * *Files identical despite different names*

### Comparing `mosamaticdesktop-1.8.0/mosamaticdesktop/tasks/createpngfromtagfiletask/createpngfromtagfiletaskwidget.py` & `mosamaticdesktop-1.9.0/mosamaticdesktop/tasks/createpngfromtagfiletask/createpngfromtagfiletaskwidget.py`

 * *Files identical despite different names*

### Comparing `mosamaticdesktop-1.8.0/mosamaticdesktop/tasks/decompressdicomtask/decompressdicomtask.py` & `mosamaticdesktop-1.9.0/mosamaticdesktop/tasks/decompressdicomtask/decompressdicomtask.py`

 * *Files identical despite different names*

### Comparing `mosamaticdesktop-1.8.0/mosamaticdesktop/tasks/decompressdicomtask/decompressdicomtaskwidget.py` & `mosamaticdesktop-1.9.0/mosamaticdesktop/tasks/decompressdicomtask/decompressdicomtaskwidget.py`

 * *Files identical despite different names*

### Comparing `mosamaticdesktop-1.8.0/mosamaticdesktop/tasks/descriptionparameter.py` & `mosamaticdesktop-1.9.0/mosamaticdesktop/tasks/descriptionparameter.py`

 * *Files identical despite different names*

### Comparing `mosamaticdesktop-1.8.0/mosamaticdesktop/tasks/dummytask/dummytask.py` & `mosamaticdesktop-1.9.0/mosamaticdesktop/tasks/dummytask/dummytask.py`

 * *Files identical despite different names*

### Comparing `mosamaticdesktop-1.8.0/mosamaticdesktop/tasks/dummytask/dummytaskwidget.py` & `mosamaticdesktop-1.9.0/mosamaticdesktop/tasks/dummytask/dummytaskwidget.py`

 * *Files identical despite different names*

### Comparing `mosamaticdesktop-1.8.0/mosamaticdesktop/tasks/filesetparameter.py` & `mosamaticdesktop-1.9.0/mosamaticdesktop/tasks/filesetparameter.py`

 * *Files identical despite different names*

### Comparing `mosamaticdesktop-1.8.0/mosamaticdesktop/tasks/floatingpointparameter.py` & `mosamaticdesktop-1.9.0/mosamaticdesktop/tasks/floatingpointparameter.py`

 * *Files identical despite different names*

### Comparing `mosamaticdesktop-1.8.0/mosamaticdesktop/tasks/integerparameter.py` & `mosamaticdesktop-1.9.0/mosamaticdesktop/tasks/integerparameter.py`

 * *Files identical despite different names*

### Comparing `mosamaticdesktop-1.8.0/mosamaticdesktop/tasks/labelparameter.py` & `mosamaticdesktop-1.9.0/mosamaticdesktop/tasks/labelparameter.py`

 * *Files identical despite different names*

### Comparing `mosamaticdesktop-1.8.0/mosamaticdesktop/tasks/multifilesetparameter.py` & `mosamaticdesktop-1.9.0/mosamaticdesktop/tasks/multifilesetparameter.py`

 * *Files identical despite different names*

### Comparing `mosamaticdesktop-1.8.0/mosamaticdesktop/tasks/musclefatsegmentationtask/musclefatsegmentationtask.py` & `mosamaticdesktop-1.9.0/mosamaticdesktop/tasks/musclefatsegmentationtask/musclefatsegmentationtask.py`

 * *Files identical despite different names*

### Comparing `mosamaticdesktop-1.8.0/mosamaticdesktop/tasks/musclefatsegmentationtask/musclefatsegmentationtaskwidget.py` & `mosamaticdesktop-1.9.0/mosamaticdesktop/tasks/musclefatsegmentationtask/musclefatsegmentationtaskwidget.py`

 * *Files identical despite different names*

### Comparing `mosamaticdesktop-1.8.0/mosamaticdesktop/tasks/optiongroupparameter.py` & `mosamaticdesktop-1.9.0/mosamaticdesktop/tasks/optiongroupparameter.py`

 * *Files identical despite different names*

### Comparing `mosamaticdesktop-1.8.0/mosamaticdesktop/tasks/parameter.py` & `mosamaticdesktop-1.9.0/mosamaticdesktop/tasks/parameter.py`

 * *Files identical despite different names*

### Comparing `mosamaticdesktop-1.8.0/mosamaticdesktop/tasks/parametercopier.py` & `mosamaticdesktop-1.9.0/mosamaticdesktop/tasks/parametercopier.py`

 * *Files identical despite different names*

### Comparing `mosamaticdesktop-1.8.0/mosamaticdesktop/tasks/pathparameter.py` & `mosamaticdesktop-1.9.0/mosamaticdesktop/tasks/pathparameter.py`

 * *Files identical despite different names*

### Comparing `mosamaticdesktop-1.8.0/mosamaticdesktop/tasks/task.py` & `mosamaticdesktop-1.9.0/mosamaticdesktop/tasks/task.py`

 * *Files identical despite different names*

### Comparing `mosamaticdesktop-1.8.0/mosamaticdesktop/tasks/taskruninfodialog.py` & `mosamaticdesktop-1.9.0/mosamaticdesktop/tasks/taskruninfodialog.py`

 * *Files identical despite different names*

### Comparing `mosamaticdesktop-1.8.0/mosamaticdesktop/tasks/taskwidget.py` & `mosamaticdesktop-1.9.0/mosamaticdesktop/tasks/taskwidget.py`

 * *Files identical despite different names*

### Comparing `mosamaticdesktop-1.8.0/mosamaticdesktop/tasks/taskwidgetmanager.py` & `mosamaticdesktop-1.9.0/mosamaticdesktop/tasks/taskwidgetmanager.py`

 * *Files identical despite different names*

### Comparing `mosamaticdesktop-1.8.0/mosamaticdesktop/tasks/taskwidgetparameterdialog.py` & `mosamaticdesktop-1.9.0/mosamaticdesktop/tasks/taskwidgetparameterdialog.py`

 * *Files identical despite different names*

### Comparing `mosamaticdesktop-1.8.0/mosamaticdesktop/tasks/textparameter.py` & `mosamaticdesktop-1.9.0/mosamaticdesktop/tasks/textparameter.py`

 * *Files identical despite different names*

### Comparing `mosamaticdesktop-1.8.0/mosamaticdesktop/utils.py` & `mosamaticdesktop-1.9.0/mosamaticdesktop/utils.py`

 * *Files identical despite different names*

### Comparing `mosamaticdesktop-1.8.0/mosamaticdesktop/widgets/datadockwidget.py` & `mosamaticdesktop-1.9.0/mosamaticdesktop/widgets/datadockwidget.py`

 * *Files identical despite different names*

### Comparing `mosamaticdesktop-1.8.0/mosamaticdesktop/widgets/dockwidget.py` & `mosamaticdesktop-1.9.0/mosamaticdesktop/widgets/dockwidget.py`

 * *Files identical despite different names*

### Comparing `mosamaticdesktop-1.8.0/mosamaticdesktop/widgets/fileitemmenu.py` & `mosamaticdesktop-1.9.0/mosamaticdesktop/widgets/fileitemmenu.py`

 * *Files identical despite different names*

### Comparing `mosamaticdesktop-1.8.0/mosamaticdesktop/widgets/filesetitem.py` & `mosamaticdesktop-1.9.0/mosamaticdesktop/widgets/filesetitem.py`

 * *Files identical despite different names*

### Comparing `mosamaticdesktop-1.8.0/mosamaticdesktop/widgets/filesetitemmenu.py` & `mosamaticdesktop-1.9.0/mosamaticdesktop/widgets/filesetitemmenu.py`

 * *Files identical despite different names*

### Comparing `mosamaticdesktop-1.8.0/mosamaticdesktop/widgets/filesettreeview.py` & `mosamaticdesktop-1.9.0/mosamaticdesktop/widgets/filesettreeview.py`

 * *Files identical despite different names*

### Comparing `mosamaticdesktop-1.8.0/mosamaticdesktop/widgets/mainviewerdockwidget.py` & `mosamaticdesktop-1.9.0/mosamaticdesktop/widgets/mainviewerdockwidget.py`

 * *Files identical despite different names*

### Comparing `mosamaticdesktop-1.8.0/mosamaticdesktop/widgets/taskdockwidget.py` & `mosamaticdesktop-1.9.0/mosamaticdesktop/widgets/taskdockwidget.py`

 * *Files identical despite different names*

### Comparing `mosamaticdesktop-1.8.0/mosamaticdesktop/widgets/viewers/dicomviewer/dicominfolayer.py` & `mosamaticdesktop-1.9.0/mosamaticdesktop/widgets/viewers/dicomviewer/dicominfolayer.py`

 * *Files identical despite different names*

### Comparing `mosamaticdesktop-1.8.0/mosamaticdesktop/widgets/viewers/dicomviewer/dicomlayer.py` & `mosamaticdesktop-1.9.0/mosamaticdesktop/widgets/viewers/dicomviewer/dicomlayer.py`

 * *Files identical despite different names*

### Comparing `mosamaticdesktop-1.8.0/mosamaticdesktop/widgets/viewers/dicomviewer/dicomviewer.py` & `mosamaticdesktop-1.9.0/mosamaticdesktop/widgets/viewers/dicomviewer/dicomviewer.py`

 * *Files identical despite different names*

### Comparing `mosamaticdesktop-1.8.0/mosamaticdesktop/widgets/viewers/dicomviewer/filesetcombobox.py` & `mosamaticdesktop-1.9.0/mosamaticdesktop/widgets/viewers/dicomviewer/filesetcombobox.py`

 * *Files identical despite different names*

### Comparing `mosamaticdesktop-1.8.0/mosamaticdesktop/widgets/viewers/dicomviewer/layer.py` & `mosamaticdesktop-1.9.0/mosamaticdesktop/widgets/viewers/dicomviewer/layer.py`

 * *Files identical despite different names*

### Comparing `mosamaticdesktop-1.8.0/mosamaticdesktop/widgets/viewers/dicomviewer/segmentationlayer.py` & `mosamaticdesktop-1.9.0/mosamaticdesktop/widgets/viewers/dicomviewer/segmentationlayer.py`

 * *Files identical despite different names*

### Comparing `mosamaticdesktop-1.8.0/mosamaticdesktop/widgets/viewers/dicomviewer/taglayer.py` & `mosamaticdesktop-1.9.0/mosamaticdesktop/widgets/viewers/dicomviewer/taglayer.py`

 * *Files identical despite different names*

### Comparing `mosamaticdesktop-1.8.0/mosamaticdesktop.egg-info/SOURCES.txt` & `mosamaticdesktop-1.9.0/mosamaticdesktop.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -77,14 +77,20 @@
 mosamaticdesktop/tasks/decompressdicomtask/decompressdicomtaskwidget.py
 mosamaticdesktop/tasks/dummytask/__init__.py
 mosamaticdesktop/tasks/dummytask/dummytask.py
 mosamaticdesktop/tasks/dummytask/dummytaskwidget.py
 mosamaticdesktop/tasks/musclefatsegmentationtask/__init__.py
 mosamaticdesktop/tasks/musclefatsegmentationtask/musclefatsegmentationtask.py
 mosamaticdesktop/tasks/musclefatsegmentationtask/musclefatsegmentationtaskwidget.py
+mosamaticdesktop/tasks/totalsegmentatorroiselectiontask/__init__.py
+mosamaticdesktop/tasks/totalsegmentatorroiselectiontask/totalsegmentatorroiselectiontask.py
+mosamaticdesktop/tasks/totalsegmentatorroiselectiontask/totalsegmentatorroiselectiontaskwidget.py
+mosamaticdesktop/tasks/totalsegmentatortask/__init__.py
+mosamaticdesktop/tasks/totalsegmentatortask/totalsegmentatortask.py
+mosamaticdesktop/tasks/totalsegmentatortask/totalsegmentatortaskwidget.py
 mosamaticdesktop/widgets/__init__.py
 mosamaticdesktop/widgets/datadockwidget.py
 mosamaticdesktop/widgets/dockwidget.py
 mosamaticdesktop/widgets/fileitem.py
 mosamaticdesktop/widgets/fileitemmenu.py
 mosamaticdesktop/widgets/filesetitem.py
 mosamaticdesktop/widgets/filesetitemmenu.py
```

### Comparing `mosamaticdesktop-1.8.0/setup.py` & `mosamaticdesktop-1.9.0/setup.py`

 * *Files identical despite different names*

