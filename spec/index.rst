Spec Home
=========

The place where all specs lives.


Project Specs
-------------

Arenadata DB (ADB)
^^^^^^^^^^^^^^^^^^^^^^^^^^^^

======= ===============================================================
Project Bundle
======= ===============================================================
TBD     `adcm_cluster_adb <https://spec.adsw.io/adcm_cluster_adb/>`_
======= ===============================================================

Arenadata Quick Marts (ADQM)
^^^^^^^^^^^^^^^^^^^^^^^^^^^^

======= ===============================================================
Project Bundle
======= ===============================================================
TBD     `adcm_cluster_adqm <https://spec.adsw.io/adcm_cluster_adqm/>`_
======= ===============================================================

Arenadata Hadoop (ADH)
^^^^^^^^^^^^^^^^^^^^^^

======= ===================================================================
Project Bundle
======= ===================================================================
TBD     `adcm_cluster_hadoop <https://spec.adsw.io/adcm_cluster_hadoop/>`_
======= ===================================================================

Arenadata Second Storage (ADSS)
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

======= =================================================================================== ================================================
Project Bundle                                                                              Application
======= =================================================================================== ================================================
TBD     `adcm_cluster_second_storage <https://spec.adsw.io/adcm_cluster_second_storage/>`_  `adss_core <https://spec.adsw.io/adss_core/>`_
======= =================================================================================== ================================================

Arenadata Monitoring (ADM)
^^^^^^^^^^^^^^^^^^^^^^^^^^

======= ==========================================================================
Project Bundle
======= ==========================================================================
TBD     `adcm_cluster_monitoring <https://spec.adsw.io/adcm_cluster_monitoring/>`_
======= ==========================================================================

Arenadata Platform Security (ADPS)
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
======= ==========================================================================================
Project Bundle
======= ==========================================================================================
TBD     `adcm_cluster_platform_security <https://spec.adsw.io/adcm_cluster_platform_security/>`_  
======= ==========================================================================================

Arenadata Streaming (ADS)
^^^^^^^^^^^^^^^^^^^^^^^^^
======= =============================================================
Project Bundle
======= =============================================================
TBD     `adcm_cluster_ads <https://spec.adsw.io/adcm_cluster_ads/>`_
======= =============================================================

Arenadata LogSearch (ADLS)
^^^^^^^^^^^^^^^^^^^^^^^^^^
======= ========================================================================
Project Bundle
======= ========================================================================
TBD     `adcm_cluster_logsearch <https://spec.adsw.io/adcm_cluster_logsearch/>`_
======= ========================================================================

Arenadata cluster manager (ADCM)
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
======= =======================================================================
Project Application
======= =======================================================================
TBD     `adcm_core <https://spec.adsw.io/adcm_core/>`_
======= =======================================================================

How to write specs
------------------

Quick start
^^^^^^^^^^^

* Create spec dir in your repo
* Go to spec dir and do the following (tested on linux only)

.. code-block:: sh

   docker run -it --rm -v $(pwd):/spec -u $(id -u ${USER}):$(id -g ${USER})  ci.arenadata.io/sphinx-autobuild /script/create_tmpl.sh

* Run autobuild server with command

.. code-block:: sh

  docker run -it --rm -v $(pwd):/spec -p 9000:9000 ci.arenadata.io/sphinx-autobuild:latest

* Open browser at `<http://127.0.0.1:9000>`_
* Open index.rst with your favorite editor ( vim :)  and start to edit
* See changes in browser

More information about syntax in `official docs <https://www.sphinx-doc.org/en/master/usage/restructuredtext/basics.html#literal-blocks>`_

More information about autobuild image in `sphinx-autobuild readme <https://github.com/arenadata/sphinx_builder>`_

.. note:: ``sphinx-versioning`` uses ``sphinx==1.4.8`` to build specs
