# Comparing `tmp/lowatt-enedis-2.2.0.tar.gz` & `tmp/lowatt-enedis-2.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lowatt-enedis-2.2.0.tar", last modified: Tue May 16 15:31:33 2023, max compression
+gzip compressed data, was "lowatt-enedis-2.2.1.tar", last modified: Mon Jun 19 08:40:19 2023, max compression
```

## Comparing `lowatt-enedis-2.2.0.tar` & `lowatt-enedis-2.2.1.tar`

### file list

```diff
@@ -1,159 +1,159 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 15:31:33.472520 lowatt-enedis-2.2.0/
--rw-r--r--   0 runner    (1001) docker     (123)      979 2023-05-16 15:31:28.000000 lowatt-enedis-2.2.0/.flake8
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 15:31:33.424520 lowatt-enedis-2.2.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 15:31:33.440520 lowatt-enedis-2.2.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     3629 2023-05-16 15:31:28.000000 lowatt-enedis-2.2.0/.github/workflows/tox.yml
--rw-r--r--   0 runner    (1001) docker     (123)    34619 2023-05-16 15:31:28.000000 lowatt-enedis-2.2.0/COPYING
--rw-r--r--   0 runner    (1001) docker     (123)      256 2023-05-16 15:31:28.000000 lowatt-enedis-2.2.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3030 2023-05-16 15:31:33.472520 lowatt-enedis-2.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2366 2023-05-16 15:31:28.000000 lowatt-enedis-2.2.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 15:31:33.444520 lowatt-enedis-2.2.0/lowatt_enedis/
--rw-r--r--   0 runner    (1001) docker     (123)    12323 2023-05-16 15:31:28.000000 lowatt-enedis-2.2.0/lowatt_enedis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2075 2023-05-16 15:31:28.000000 lowatt-enedis-2.2.0/lowatt_enedis/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2839 2023-05-16 15:31:28.000000 lowatt-enedis-2.2.0/lowatt_enedis/certauth.py
--rw-r--r--   0 runner    (1001) docker     (123)    31440 2023-05-16 15:31:28.000000 lowatt-enedis-2.2.0/lowatt_enedis/services.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 15:31:33.436520 lowatt-enedis-2.2.0/lowatt_enedis/wsdl/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 15:31:33.424520 lowatt-enedis-2.2.0/lowatt_enedis/wsdl/CommandeAccesDonneesMesures/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 15:31:33.424520 lowatt-enedis-2.2.0/lowatt_enedis/wsdl/CommandeAccesDonneesMesures/Services/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 15:31:33.448520 lowatt-enedis-2.2.0/lowatt_enedis/wsdl/CommandeAccesDonneesMesures/Services/CommanderAccesDonneesMesures/
--rw-r--r--   0 runner    (1001) docker     (123)     3993 2023-05-16 15:31:28.000000 lowatt-enedis-2.2.0/lowatt_enedis/wsdl/CommandeAccesDonneesMesures/Services/CommanderAccesDonneesMesures/CommanderAccesDonneesMesures-V1.0.wsdl
--rw-r--r--   0 runner    (1001) docker     (123)     9179 2023-05-16 15:31:28.000000 lowatt-enedis-2.2.0/lowatt_enedis/wsdl/CommandeAccesDonneesMesures/Services/CommanderAccesDonneesMesures/CommanderAccesDonneesMesures-V1.0.xsd
--rw-r--r--   0 runner    (1001) docker     (123)     4835 2023-05-16 15:31:28.000000 lowatt-enedis-2.2.0/lowatt_enedis/wsdl/CommandeAccesDonneesMesures/Services/CommanderAccesDonneesMesures/ENEDIS.Dictionnaire.Technique.v1.0.xsd
--rw-r--r--   0 runner    (1001) docker     (123)    42043 2023-05-16 15:31:28.000000 lowatt-enedis-2.2.0/lowatt_enedis/wsdl/CommandeAccesDonneesMesures/Services/CommanderAccesDonneesMesures/ENEDIS.Dictionnaire.TypeComplexe.v5.0.xsd
--rw-r--r--   0 runner    (1001) docker     (123)    45741 2023-05-16 15:31:28.000000 lowatt-enedis-2.2.0/lowatt_enedis/wsdl/CommandeAccesDonneesMesures/Services/CommanderAccesDonneesMesures/ENEDIS.Dictionnaire.TypeSimple.v5.0.xsd
--rw-r--r--   0 runner    (1001) docker     (123)     6426 2023-05-16 15:31:28.000000 lowatt-enedis-2.2.0/lowatt_enedis/wsdl/CommandeAccesDonneesMesures/Services/CommanderAccesDonneesMesures/W3C.SoapEnv.xsd
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 15:31:33.424520 lowatt-enedis-2.2.0/lowatt_enedis/wsdl/CommandeArretServiceSouscritMesures/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 15:31:33.424520 lowatt-enedis-2.2.0/lowatt_enedis/wsdl/CommandeArretServiceSouscritMesures/Dictionnaires/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 15:31:33.424520 lowatt-enedis-2.2.0/lowatt_enedis/wsdl/CommandeArretServiceSouscritMesures/Dictionnaires/Metier/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 15:31:33.448520 lowatt-enedis-2.2.0/lowatt_enedis/wsdl/CommandeArretServiceSouscritMesures/Dictionnaires/Metier/v5.0/
--rw-r--r--   0 runner    (1001) docker     (123)    36631 2023-05-16 15:31:28.000000 lowatt-enedis-2.2.0/lowatt_enedis/wsdl/CommandeArretServiceSouscritMesures/Dictionnaires/Metier/v5.0/ENEDIS.Dictionnaire.TypeComplexe.v5.0.xsd
--rw-r--r--   0 runner    (1001) docker     (123)    37127 2023-05-16 15:31:28.000000 lowatt-enedis-2.2.0/lowatt_enedis/wsdl/CommandeArretServiceSouscritMesures/Dictionnaires/Metier/v5.0/ENEDIS.Dictionnaire.TypeSimple.v5.0.xsd
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 15:31:33.448520 lowatt-enedis-2.2.0/lowatt_enedis/wsdl/CommandeArretServiceSouscritMesures/Dictionnaires/Technique/
--rw-r--r--   0 runner    (1001) docker     (123)     3201 2023-05-16 15:31:28.000000 lowatt-enedis-2.2.0/lowatt_enedis/wsdl/CommandeArretServiceSouscritMesures/Dictionnaires/Technique/W3C.SoapEnv.xsd
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 15:31:33.448520 lowatt-enedis-2.2.0/lowatt_enedis/wsdl/CommandeArretServiceSouscritMesures/Dictionnaires/Technique/v1.0/
--rw-r--r--   0 runner    (1001) docker     (123)     4276 2023-05-16 15:31:28.000000 lowatt-enedis-2.2.0/lowatt_enedis/wsdl/CommandeArretServiceSouscritMesures/Dictionnaires/Technique/v1.0/ENEDIS.Dictionnaire.Technique.v1.0.xsd
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 15:31:33.424520 lowatt-enedis-2.2.0/lowatt_enedis/wsdl/CommandeArretServiceSouscritMesures/Services/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 15:31:33.448520 lowatt-enedis-2.2.0/lowatt_enedis/wsdl/CommandeArretServiceSouscritMesures/Services/CommandeArretServiceSouscritMesures/
--rw-r--r--   0 runner    (1001) docker     (123)     3851 2023-05-16 15:31:28.000000 lowatt-enedis-2.2.0/lowatt_enedis/wsdl/CommandeArretServiceSouscritMesures/Services/CommandeArretServiceSouscritMesures/CommandeArretServiceSouscritMesures-v1.0.wsdl
--rw-r--r--   0 runner    (1001) docker     (123)     2921 2023-05-16 15:31:28.000000 lowatt-enedis-2.2.0/lowatt_enedis/wsdl/CommandeArretServiceSouscritMesures/Services/CommandeArretServiceSouscritMesures/CommanderArretServiceSouscritMesures-v1.0.xsd
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 15:31:33.428520 lowatt-enedis-2.2.0/lowatt_enedis/wsdl/CommandeCollectePublicationMesures/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 15:31:33.428520 lowatt-enedis-2.2.0/lowatt_enedis/wsdl/CommandeCollectePublicationMesures/Dictionnaires/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 15:31:33.428520 lowatt-enedis-2.2.0/lowatt_enedis/wsdl/CommandeCollectePublicationMesures/Dictionnaires/Metier/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 15:31:33.452520 lowatt-enedis-2.2.0/lowatt_enedis/wsdl/CommandeCollectePublicationMesures/Dictionnaires/Metier/v5.0/
--rw-r--r--   0 runner    (1001) docker     (123)    36631 2023-05-16 15:31:28.000000 lowatt-enedis-2.2.0/lowatt_enedis/wsdl/CommandeCollectePublicationMesures/Dictionnaires/Metier/v5.0/ENEDIS.Dictionnaire.TypeComplexe.v5.0.xsd
--rw-r--r--   0 runner    (1001) docker     (123)    37127 2023-05-16 15:31:28.000000 lowatt-enedis-2.2.0/lowatt_enedis/wsdl/CommandeCollectePublicationMesures/Dictionnaires/Metier/v5.0/ENEDIS.Dictionnaire.TypeSimple.v5.0.xsd
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 15:31:33.452520 lowatt-enedis-2.2.0/lowatt_enedis/wsdl/CommandeCollectePublicationMesures/Dictionnaires/Technique/
--rw-r--r--   0 runner    (1001) docker     (123)     3201 2023-05-16 15:31:28.000000 lowatt-enedis-2.2.0/lowatt_enedis/wsdl/CommandeCollectePublicationMesures/Dictionnaires/Technique/W3C.SoapEnv.xsd
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 15:31:33.452520 lowatt-enedis-2.2.0/lowatt_enedis/wsdl/CommandeCollectePublicationMesures/Dictionnaires/Technique/v1.0/
--rw-r--r--   0 runner    (1001) docker     (123)     4276 2023-05-16 15:31:28.000000 lowatt-enedis-2.2.0/lowatt_enedis/wsdl/CommandeCollectePublicationMesures/Dictionnaires/Technique/v1.0/ENEDIS.Dictionnaire.Technique.v1.0.xsd
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 15:31:33.428520 lowatt-enedis-2.2.0/lowatt_enedis/wsdl/CommandeCollectePublicationMesures/Services/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 15:31:33.452520 lowatt-enedis-2.2.0/lowatt_enedis/wsdl/CommandeCollectePublicationMesures/Services/CommandeCollectePublicationMesures/
--rw-r--r--   0 runner    (1001) docker     (123)     3653 2023-05-16 15:31:28.000000 lowatt-enedis-2.2.0/lowatt_enedis/wsdl/CommandeCollectePublicationMesures/Services/CommandeCollectePublicationMesures/CommandeCollectePublicationMesures-v3.0.wsdl
--rw-r--r--   0 runner    (1001) docker     (123)     4467 2023-05-16 15:31:28.000000 lowatt-enedis-2.2.0/lowatt_enedis/wsdl/CommandeCollectePublicationMesures/Services/CommandeCollectePublicationMesures/CommanderCollectePublicationMesures-v3.0.xsd
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 15:31:33.428520 lowatt-enedis-2.2.0/lowatt_enedis/wsdl/CommandeTransmissionDonneesInfraJ/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 15:31:33.428520 lowatt-enedis-2.2.0/lowatt_enedis/wsdl/CommandeTransmissionDonneesInfraJ/Dictionnaires/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 15:31:33.428520 lowatt-enedis-2.2.0/lowatt_enedis/wsdl/CommandeTransmissionDonneesInfraJ/Dictionnaires/Metier/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 15:31:33.452520 lowatt-enedis-2.2.0/lowatt_enedis/wsdl/CommandeTransmissionDonneesInfraJ/Dictionnaires/Metier/v5.0/
--rw-r--r--   0 runner    (1001) docker     (123)    37212 2023-05-16 15:31:28.000000 lowatt-enedis-2.2.0/lowatt_enedis/wsdl/CommandeTransmissionDonneesInfraJ/Dictionnaires/Metier/v5.0/ENEDIS.Dictionnaire.TypeComplexe.v5.0.xsd
--rw-r--r--   0 runner    (1001) docker     (123)    38245 2023-05-16 15:31:28.000000 lowatt-enedis-2.2.0/lowatt_enedis/wsdl/CommandeTransmissionDonneesInfraJ/Dictionnaires/Metier/v5.0/ENEDIS.Dictionnaire.TypeSimple.v5.0.xsd
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 15:31:33.452520 lowatt-enedis-2.2.0/lowatt_enedis/wsdl/CommandeTransmissionDonneesInfraJ/Dictionnaires/Technique/
--rw-r--r--   0 runner    (1001) docker     (123)     3201 2023-05-16 15:31:28.000000 lowatt-enedis-2.2.0/lowatt_enedis/wsdl/CommandeTransmissionDonneesInfraJ/Dictionnaires/Technique/W3C.SoapEnv.xsd
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 15:31:33.452520 lowatt-enedis-2.2.0/lowatt_enedis/wsdl/CommandeTransmissionDonneesInfraJ/Dictionnaires/Technique/v1.0/
--rw-r--r--   0 runner    (1001) docker     (123)     4276 2023-05-16 15:31:28.000000 lowatt-enedis-2.2.0/lowatt_enedis/wsdl/CommandeTransmissionDonneesInfraJ/Dictionnaires/Technique/v1.0/ENEDIS.Dictionnaire.Technique.v1.0.xsd
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 15:31:33.432520 lowatt-enedis-2.2.0/lowatt_enedis/wsdl/CommandeTransmissionDonneesInfraJ/Services/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 15:31:33.452520 lowatt-enedis-2.2.0/lowatt_enedis/wsdl/CommandeTransmissionDonneesInfraJ/Services/CommandeTransmissionDonneesInfraJ/
--rw-r--r--   0 runner    (1001) docker     (123)     3638 2023-05-16 15:31:28.000000 lowatt-enedis-2.2.0/lowatt_enedis/wsdl/CommandeTransmissionDonneesInfraJ/Services/CommandeTransmissionDonneesInfraJ/CommandeTransmissionDonneesInfraJ-v1.0.wsdl
--rw-r--r--   0 runner    (1001) docker     (123)     4028 2023-05-16 15:31:28.000000 lowatt-enedis-2.2.0/lowatt_enedis/wsdl/CommandeTransmissionDonneesInfraJ/Services/CommandeTransmissionDonneesInfraJ/CommanderTransmissionDonneesInfraJ-v1.0.xsd
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 15:31:33.432520 lowatt-enedis-2.2.0/lowatt_enedis/wsdl/ConsultationDonneesTechniquesContractuelles/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 15:31:33.432520 lowatt-enedis-2.2.0/lowatt_enedis/wsdl/ConsultationDonneesTechniquesContractuelles/Dictionnaire/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 15:31:33.432520 lowatt-enedis-2.2.0/lowatt_enedis/wsdl/ConsultationDonneesTechniquesContractuelles/Dictionnaire/Metier/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 15:31:33.456520 lowatt-enedis-2.2.0/lowatt_enedis/wsdl/ConsultationDonneesTechniquesContractuelles/Dictionnaire/Metier/v5.0/
--rw-r--r--   0 runner    (1001) docker     (123)    37450 2023-05-16 15:31:28.000000 lowatt-enedis-2.2.0/lowatt_enedis/wsdl/ConsultationDonneesTechniquesContractuelles/Dictionnaire/Metier/v5.0/ENEDIS.Dictionnaire.TypeComplexe.v5.0.xsd
--rw-r--r--   0 runner    (1001) docker     (123)    38416 2023-05-16 15:31:28.000000 lowatt-enedis-2.2.0/lowatt_enedis/wsdl/ConsultationDonneesTechniquesContractuelles/Dictionnaire/Metier/v5.0/ENEDIS.Dictionnaire.TypeSimple.v5.0.xsd
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 15:31:33.456520 lowatt-enedis-2.2.0/lowatt_enedis/wsdl/ConsultationDonneesTechniquesContractuelles/Dictionnaire/Technique/
--rw-r--r--   0 runner    (1001) docker     (123)     4234 2023-05-16 15:31:28.000000 lowatt-enedis-2.2.0/lowatt_enedis/wsdl/ConsultationDonneesTechniquesContractuelles/Dictionnaire/Technique/ENEDIS.Dictionnaire.Technique.v1.0.xsd
--rw-r--r--   0 runner    (1001) docker     (123)     6061 2023-05-16 15:31:28.000000 lowatt-enedis-2.2.0/lowatt_enedis/wsdl/ConsultationDonneesTechniquesContractuelles/Dictionnaire/Technique/W3C.SoapEnv.xsd
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 15:31:33.432520 lowatt-enedis-2.2.0/lowatt_enedis/wsdl/ConsultationDonneesTechniquesContractuelles/Services/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 15:31:33.456520 lowatt-enedis-2.2.0/lowatt_enedis/wsdl/ConsultationDonneesTechniquesContractuelles/Services/ConsultationDonneesTechniquesContractuelles/
--rw-r--r--   0 runner    (1001) docker     (123)     3602 2023-05-16 15:31:28.000000 lowatt-enedis-2.2.0/lowatt_enedis/wsdl/ConsultationDonneesTechniquesContractuelles/Services/ConsultationDonneesTechniquesContractuelles/ConsultationDonneesTechniquesContractuelles-v1.0.wsdl
--rw-r--r--   0 runner    (1001) docker     (123)    11723 2023-05-16 15:31:28.000000 lowatt-enedis-2.2.0/lowatt_enedis/wsdl/ConsultationDonneesTechniquesContractuelles/Services/ConsultationDonneesTechniquesContractuelles/ConsulterDonneesTechniquesContractuelles-v1.0.xsd
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 15:31:33.432520 lowatt-enedis-2.2.0/lowatt_enedis/wsdl/ConsultationMesures/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 15:31:33.432520 lowatt-enedis-2.2.0/lowatt_enedis/wsdl/ConsultationMesures/Dictionnaires/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 15:31:33.432520 lowatt-enedis-2.2.0/lowatt_enedis/wsdl/ConsultationMesures/Dictionnaires/Metier/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 15:31:33.456520 lowatt-enedis-2.2.0/lowatt_enedis/wsdl/ConsultationMesures/Dictionnaires/Metier/v5.0/
--rw-r--r--   0 runner    (1001) docker     (123)    37450 2023-05-16 15:31:28.000000 lowatt-enedis-2.2.0/lowatt_enedis/wsdl/ConsultationMesures/Dictionnaires/Metier/v5.0/ENEDIS.Dictionnaire.TypeComplexe.v5.0.xsd
--rw-r--r--   0 runner    (1001) docker     (123)    38224 2023-05-16 15:31:28.000000 lowatt-enedis-2.2.0/lowatt_enedis/wsdl/ConsultationMesures/Dictionnaires/Metier/v5.0/ENEDIS.Dictionnaire.TypeSimple.v5.0.xsd
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 15:31:33.456520 lowatt-enedis-2.2.0/lowatt_enedis/wsdl/ConsultationMesures/Dictionnaires/Technique/
--rw-r--r--   0 runner    (1001) docker     (123)     6061 2023-05-16 15:31:28.000000 lowatt-enedis-2.2.0/lowatt_enedis/wsdl/ConsultationMesures/Dictionnaires/Technique/W3C.SoapEnv.xsd
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 15:31:33.460520 lowatt-enedis-2.2.0/lowatt_enedis/wsdl/ConsultationMesures/Dictionnaires/Technique/v1.0/
--rw-r--r--   0 runner    (1001) docker     (123)     4373 2023-05-16 15:31:28.000000 lowatt-enedis-2.2.0/lowatt_enedis/wsdl/ConsultationMesures/Dictionnaires/Technique/v1.0/ENEDIS.Dictionnaire.Technique.v1.0.xsd
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 15:31:33.432520 lowatt-enedis-2.2.0/lowatt_enedis/wsdl/ConsultationMesures/Services/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 15:31:33.460520 lowatt-enedis-2.2.0/lowatt_enedis/wsdl/ConsultationMesures/Services/ConsultationMesures/
--rw-r--r--   0 runner    (1001) docker     (123)     2939 2023-05-16 15:31:28.000000 lowatt-enedis-2.2.0/lowatt_enedis/wsdl/ConsultationMesures/Services/ConsultationMesures/ConsultationMesures-v1.1.wsdl
--rw-r--r--   0 runner    (1001) docker     (123)     3083 2023-05-16 15:31:28.000000 lowatt-enedis-2.2.0/lowatt_enedis/wsdl/ConsultationMesures/Services/ConsultationMesures/ConsulterMesures-v1.1.xsd
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 15:31:33.460520 lowatt-enedis-2.2.0/lowatt_enedis/wsdl/ConsultationMesuresDetaillees/
--rw-r--r--   0 runner    (1001) docker     (123)     2652 2023-05-16 15:31:28.000000 lowatt-enedis-2.2.0/lowatt_enedis/wsdl/ConsultationMesuresDetaillees/ConsultationMesuresDetaillees-v2.0.wsdl
--rw-r--r--   0 runner    (1001) docker     (123)     3793 2023-05-16 15:31:28.000000 lowatt-enedis-2.2.0/lowatt_enedis/wsdl/ConsultationMesuresDetaillees/ConsulterMesuresDetaillees-v2.0.1.xsd
--rw-r--r--   0 runner    (1001) docker     (123)     4234 2023-05-16 15:31:28.000000 lowatt-enedis-2.2.0/lowatt_enedis/wsdl/ConsultationMesuresDetaillees/ENEDIS.Dictionnaire.Technique.v1.0.xsd
--rw-r--r--   0 runner    (1001) docker     (123)     6177 2023-05-16 15:31:28.000000 lowatt-enedis-2.2.0/lowatt_enedis/wsdl/ConsultationMesuresDetaillees/W3C.SoapEnv.xsd
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 15:31:33.460520 lowatt-enedis-2.2.0/lowatt_enedis/wsdl/ConsultationMesuresDetailleesV3/
--rw-r--r--   0 runner    (1001) docker     (123)    11126 2023-05-16 15:31:28.000000 lowatt-enedis-2.2.0/lowatt_enedis/wsdl/ConsultationMesuresDetailleesV3/ADAM.ConsulterMesuresDetailleesCommun.xsd
--rw-r--r--   0 runner    (1001) docker     (123)     2977 2023-05-16 15:31:28.000000 lowatt-enedis-2.2.0/lowatt_enedis/wsdl/ConsultationMesuresDetailleesV3/ConsultationMesuresDetaillees-v3.0.wsdl
--rw-r--r--   0 runner    (1001) docker     (123)     4835 2023-05-16 15:31:28.000000 lowatt-enedis-2.2.0/lowatt_enedis/wsdl/ConsultationMesuresDetailleesV3/ENEDIS.Dictionnaire.Technique.v1.0.xsd
--rw-r--r--   0 runner    (1001) docker     (123)     6426 2023-05-16 15:31:28.000000 lowatt-enedis-2.2.0/lowatt_enedis/wsdl/ConsultationMesuresDetailleesV3/W3C.SoapEnv.xsd
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 15:31:33.436520 lowatt-enedis-2.2.0/lowatt_enedis/wsdl/RecherchePoint/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 15:31:33.436520 lowatt-enedis-2.2.0/lowatt_enedis/wsdl/RecherchePoint/Dictionnaires/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 15:31:33.464520 lowatt-enedis-2.2.0/lowatt_enedis/wsdl/RecherchePoint/Dictionnaires/Technique/
--rw-r--r--   0 runner    (1001) docker     (123)     4328 2023-05-16 15:31:28.000000 lowatt-enedis-2.2.0/lowatt_enedis/wsdl/RecherchePoint/Dictionnaires/Technique/ENEDIS.Dictionnaire.Technique.v1.0.xsd
--rw-r--r--   0 runner    (1001) docker     (123)     6177 2023-05-16 15:31:28.000000 lowatt-enedis-2.2.0/lowatt_enedis/wsdl/RecherchePoint/Dictionnaires/Technique/W3C.SoapEnv.xsd
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 15:31:33.464520 lowatt-enedis-2.2.0/lowatt_enedis/wsdl/RecherchePoint/Dictionnaires/v5.0/
--rw-r--r--   0 runner    (1001) docker     (123)    37450 2023-05-16 15:31:28.000000 lowatt-enedis-2.2.0/lowatt_enedis/wsdl/RecherchePoint/Dictionnaires/v5.0/ENEDIS.Dictionnaire.TypeComplexe.v5.0.xsd
--rw-r--r--   0 runner    (1001) docker     (123)    38452 2023-05-16 15:31:28.000000 lowatt-enedis-2.2.0/lowatt_enedis/wsdl/RecherchePoint/Dictionnaires/v5.0/ENEDIS.Dictionnaire.TypeSimple.v5.0.xsd
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 15:31:33.436520 lowatt-enedis-2.2.0/lowatt_enedis/wsdl/RecherchePoint/Services/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 15:31:33.464520 lowatt-enedis-2.2.0/lowatt_enedis/wsdl/RecherchePoint/Services/RecherchePoint/
--rw-r--r--   0 runner    (1001) docker     (123)     2872 2023-05-16 15:31:28.000000 lowatt-enedis-2.2.0/lowatt_enedis/wsdl/RecherchePoint/Services/RecherchePoint/RecherchePoint-v2.0.wsdl
--rw-r--r--   0 runner    (1001) docker     (123)     3467 2023-05-16 15:31:28.000000 lowatt-enedis-2.2.0/lowatt_enedis/wsdl/RecherchePoint/Services/RecherchePoint/RechercherPoint-v2.0.xsd
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 15:31:33.436520 lowatt-enedis-2.2.0/lowatt_enedis/wsdl/RechercheServicesSouscritsMesures/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 15:31:33.436520 lowatt-enedis-2.2.0/lowatt_enedis/wsdl/RechercheServicesSouscritsMesures/Dictionnaires/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 15:31:33.436520 lowatt-enedis-2.2.0/lowatt_enedis/wsdl/RechercheServicesSouscritsMesures/Dictionnaires/Metier/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 15:31:33.464520 lowatt-enedis-2.2.0/lowatt_enedis/wsdl/RechercheServicesSouscritsMesures/Dictionnaires/Metier/v5.0/
--rw-r--r--   0 runner    (1001) docker     (123)    37212 2023-05-16 15:31:28.000000 lowatt-enedis-2.2.0/lowatt_enedis/wsdl/RechercheServicesSouscritsMesures/Dictionnaires/Metier/v5.0/ENEDIS.Dictionnaire.TypeComplexe.v5.0.xsd
--rw-r--r--   0 runner    (1001) docker     (123)    38245 2023-05-16 15:31:28.000000 lowatt-enedis-2.2.0/lowatt_enedis/wsdl/RechercheServicesSouscritsMesures/Dictionnaires/Metier/v5.0/ENEDIS.Dictionnaire.TypeSimple.v5.0.xsd
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 15:31:33.464520 lowatt-enedis-2.2.0/lowatt_enedis/wsdl/RechercheServicesSouscritsMesures/Dictionnaires/Technique/
--rw-r--r--   0 runner    (1001) docker     (123)     3062 2023-05-16 15:31:28.000000 lowatt-enedis-2.2.0/lowatt_enedis/wsdl/RechercheServicesSouscritsMesures/Dictionnaires/Technique/W3C.SoapEnv.xsd
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 15:31:33.464520 lowatt-enedis-2.2.0/lowatt_enedis/wsdl/RechercheServicesSouscritsMesures/Dictionnaires/Technique/v1.0/
--rw-r--r--   0 runner    (1001) docker     (123)     4025 2023-05-16 15:31:28.000000 lowatt-enedis-2.2.0/lowatt_enedis/wsdl/RechercheServicesSouscritsMesures/Dictionnaires/Technique/v1.0/ENEDIS.Dictionnaire.Technique.v1.0.xsd
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 15:31:33.436520 lowatt-enedis-2.2.0/lowatt_enedis/wsdl/RechercheServicesSouscritsMesures/Services/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 15:31:33.468520 lowatt-enedis-2.2.0/lowatt_enedis/wsdl/RechercheServicesSouscritsMesures/Services/RechercheServicesSouscritsMesures/
--rw-r--r--   0 runner    (1001) docker     (123)     3321 2023-05-16 15:31:28.000000 lowatt-enedis-2.2.0/lowatt_enedis/wsdl/RechercheServicesSouscritsMesures/Services/RechercheServicesSouscritsMesures/RechercherServicesSouscritsMesures-v1.0.wsdl
--rw-r--r--   0 runner    (1001) docker     (123)     3423 2023-05-16 15:31:28.000000 lowatt-enedis-2.2.0/lowatt_enedis/wsdl/RechercheServicesSouscritsMesures/Services/RechercheServicesSouscritsMesures/RechercherServicesSouscritsMesures-v1.0.xsd
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 15:31:33.436520 lowatt-enedis-2.2.0/lowatt_enedis/wsdl/TransmissionHistoriqueMesures/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 15:31:33.436520 lowatt-enedis-2.2.0/lowatt_enedis/wsdl/TransmissionHistoriqueMesures/Dictionnaires/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 15:31:33.468520 lowatt-enedis-2.2.0/lowatt_enedis/wsdl/TransmissionHistoriqueMesures/Dictionnaires/v4.0/
--rw-r--r--   0 runner    (1001) docker     (123)    40590 2023-05-16 15:31:28.000000 lowatt-enedis-2.2.0/lowatt_enedis/wsdl/TransmissionHistoriqueMesures/Dictionnaires/v4.0/ERDF.Dictionnaire.TypeComplexe.v4.0.xsd
--rw-r--r--   0 runner    (1001) docker     (123)    36163 2023-05-16 15:31:28.000000 lowatt-enedis-2.2.0/lowatt_enedis/wsdl/TransmissionHistoriqueMesures/Dictionnaires/v4.0/ERDF.Dictionnaire.TypeSimple.v4.0.xsd
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 15:31:33.436520 lowatt-enedis-2.2.0/lowatt_enedis/wsdl/TransmissionHistoriqueMesures/Services/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 15:31:33.468520 lowatt-enedis-2.2.0/lowatt_enedis/wsdl/TransmissionHistoriqueMesures/Services/TransmissionHistoriqueMesures/
--rw-r--r--   0 runner    (1001) docker     (123)     3514 2023-05-16 15:31:28.000000 lowatt-enedis-2.2.0/lowatt_enedis/wsdl/TransmissionHistoriqueMesures/Services/TransmissionHistoriqueMesures/CommandeTransmissionHistoriqueMesures-v1.0.wsdl
--rw-r--r--   0 runner    (1001) docker     (123)     4704 2023-05-16 15:31:28.000000 lowatt-enedis-2.2.0/lowatt_enedis/wsdl/TransmissionHistoriqueMesures/Services/TransmissionHistoriqueMesures/CommanderTransmissionHistoriqueMesures-v1.0.xsd
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 15:31:33.444520 lowatt-enedis-2.2.0/lowatt_enedis.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3030 2023-05-16 15:31:33.000000 lowatt-enedis-2.2.0/lowatt_enedis.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7414 2023-05-16 15:31:33.000000 lowatt-enedis-2.2.0/lowatt_enedis.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-16 15:31:33.000000 lowatt-enedis-2.2.0/lowatt_enedis.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-05-16 15:31:33.000000 lowatt-enedis-2.2.0/lowatt_enedis.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      156 2023-05-16 15:31:33.000000 lowatt-enedis-2.2.0/lowatt_enedis.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-16 15:31:33.000000 lowatt-enedis-2.2.0/lowatt_enedis.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      227 2023-05-16 15:31:28.000000 lowatt-enedis-2.2.0/mypy.ini
--rw-r--r--   0 runner    (1001) docker     (123)      242 2023-05-16 15:31:28.000000 lowatt-enedis-2.2.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-05-16 15:31:28.000000 lowatt-enedis-2.2.0/pytest.ini
--rw-r--r--   0 runner    (1001) docker     (123)      995 2023-05-16 15:31:33.472520 lowatt-enedis-2.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      669 2023-05-16 15:31:28.000000 lowatt-enedis-2.2.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 15:31:33.468520 lowatt-enedis-2.2.0/test/
--rw-r--r--   0 runner    (1001) docker     (123)      421 2023-05-16 15:31:28.000000 lowatt-enedis-2.2.0/test/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 15:31:33.472520 lowatt-enedis-2.2.0/test/data/
--rw-r--r--   0 runner    (1001) docker     (123)     1319 2023-05-16 15:31:28.000000 lowatt-enedis-2.2.0/test/data/consulterMesuresDetailleesResponse.xml
--rw-r--r--   0 runner    (1001) docker     (123)     4247 2023-05-16 15:31:28.000000 lowatt-enedis-2.2.0/test/data/consulterMesuresResponse.xml
--rw-r--r--   0 runner    (1001) docker     (123)    92977 2023-05-16 15:31:28.000000 lowatt-enedis-2.2.0/test/data/requests.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     5804 2023-05-16 15:31:28.000000 lowatt-enedis-2.2.0/test/test_lowatt_enedis.py
--rw-r--r--   0 runner    (1001) docker     (123)     4863 2023-05-16 15:31:28.000000 lowatt-enedis-2.2.0/test/test_requests.py
--rw-r--r--   0 runner    (1001) docker     (123)      815 2023-05-16 15:31:28.000000 lowatt-enedis-2.2.0/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 08:40:19.658424 lowatt-enedis-2.2.1/
+-rw-r--r--   0 runner    (1001) docker     (123)      979 2023-06-19 08:40:11.000000 lowatt-enedis-2.2.1/.flake8
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 08:40:19.594424 lowatt-enedis-2.2.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 08:40:19.606424 lowatt-enedis-2.2.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     3629 2023-06-19 08:40:11.000000 lowatt-enedis-2.2.1/.github/workflows/tox.yml
+-rw-r--r--   0 runner    (1001) docker     (123)    34619 2023-06-19 08:40:11.000000 lowatt-enedis-2.2.1/COPYING
+-rw-r--r--   0 runner    (1001) docker     (123)      256 2023-06-19 08:40:11.000000 lowatt-enedis-2.2.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3030 2023-06-19 08:40:19.658424 lowatt-enedis-2.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2366 2023-06-19 08:40:11.000000 lowatt-enedis-2.2.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 08:40:19.610424 lowatt-enedis-2.2.1/lowatt_enedis/
+-rw-r--r--   0 runner    (1001) docker     (123)    12323 2023-06-19 08:40:11.000000 lowatt-enedis-2.2.1/lowatt_enedis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2075 2023-06-19 08:40:11.000000 lowatt-enedis-2.2.1/lowatt_enedis/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2948 2023-06-19 08:40:11.000000 lowatt-enedis-2.2.1/lowatt_enedis/certauth.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31440 2023-06-19 08:40:11.000000 lowatt-enedis-2.2.1/lowatt_enedis/services.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 08:40:19.602424 lowatt-enedis-2.2.1/lowatt_enedis/wsdl/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 08:40:19.594424 lowatt-enedis-2.2.1/lowatt_enedis/wsdl/CommandeAccesDonneesMesures/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 08:40:19.594424 lowatt-enedis-2.2.1/lowatt_enedis/wsdl/CommandeAccesDonneesMesures/Services/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 08:40:19.618424 lowatt-enedis-2.2.1/lowatt_enedis/wsdl/CommandeAccesDonneesMesures/Services/CommanderAccesDonneesMesures/
+-rw-r--r--   0 runner    (1001) docker     (123)     3993 2023-06-19 08:40:11.000000 lowatt-enedis-2.2.1/lowatt_enedis/wsdl/CommandeAccesDonneesMesures/Services/CommanderAccesDonneesMesures/CommanderAccesDonneesMesures-V1.0.wsdl
+-rw-r--r--   0 runner    (1001) docker     (123)     9179 2023-06-19 08:40:11.000000 lowatt-enedis-2.2.1/lowatt_enedis/wsdl/CommandeAccesDonneesMesures/Services/CommanderAccesDonneesMesures/CommanderAccesDonneesMesures-V1.0.xsd
+-rw-r--r--   0 runner    (1001) docker     (123)     4835 2023-06-19 08:40:11.000000 lowatt-enedis-2.2.1/lowatt_enedis/wsdl/CommandeAccesDonneesMesures/Services/CommanderAccesDonneesMesures/ENEDIS.Dictionnaire.Technique.v1.0.xsd
+-rw-r--r--   0 runner    (1001) docker     (123)    42043 2023-06-19 08:40:11.000000 lowatt-enedis-2.2.1/lowatt_enedis/wsdl/CommandeAccesDonneesMesures/Services/CommanderAccesDonneesMesures/ENEDIS.Dictionnaire.TypeComplexe.v5.0.xsd
+-rw-r--r--   0 runner    (1001) docker     (123)    45741 2023-06-19 08:40:11.000000 lowatt-enedis-2.2.1/lowatt_enedis/wsdl/CommandeAccesDonneesMesures/Services/CommanderAccesDonneesMesures/ENEDIS.Dictionnaire.TypeSimple.v5.0.xsd
+-rw-r--r--   0 runner    (1001) docker     (123)     6426 2023-06-19 08:40:11.000000 lowatt-enedis-2.2.1/lowatt_enedis/wsdl/CommandeAccesDonneesMesures/Services/CommanderAccesDonneesMesures/W3C.SoapEnv.xsd
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 08:40:19.594424 lowatt-enedis-2.2.1/lowatt_enedis/wsdl/CommandeArretServiceSouscritMesures/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 08:40:19.594424 lowatt-enedis-2.2.1/lowatt_enedis/wsdl/CommandeArretServiceSouscritMesures/Dictionnaires/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 08:40:19.594424 lowatt-enedis-2.2.1/lowatt_enedis/wsdl/CommandeArretServiceSouscritMesures/Dictionnaires/Metier/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 08:40:19.618424 lowatt-enedis-2.2.1/lowatt_enedis/wsdl/CommandeArretServiceSouscritMesures/Dictionnaires/Metier/v5.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    36631 2023-06-19 08:40:11.000000 lowatt-enedis-2.2.1/lowatt_enedis/wsdl/CommandeArretServiceSouscritMesures/Dictionnaires/Metier/v5.0/ENEDIS.Dictionnaire.TypeComplexe.v5.0.xsd
+-rw-r--r--   0 runner    (1001) docker     (123)    37127 2023-06-19 08:40:11.000000 lowatt-enedis-2.2.1/lowatt_enedis/wsdl/CommandeArretServiceSouscritMesures/Dictionnaires/Metier/v5.0/ENEDIS.Dictionnaire.TypeSimple.v5.0.xsd
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 08:40:19.618424 lowatt-enedis-2.2.1/lowatt_enedis/wsdl/CommandeArretServiceSouscritMesures/Dictionnaires/Technique/
+-rw-r--r--   0 runner    (1001) docker     (123)     3201 2023-06-19 08:40:11.000000 lowatt-enedis-2.2.1/lowatt_enedis/wsdl/CommandeArretServiceSouscritMesures/Dictionnaires/Technique/W3C.SoapEnv.xsd
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 08:40:19.622424 lowatt-enedis-2.2.1/lowatt_enedis/wsdl/CommandeArretServiceSouscritMesures/Dictionnaires/Technique/v1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     4276 2023-06-19 08:40:11.000000 lowatt-enedis-2.2.1/lowatt_enedis/wsdl/CommandeArretServiceSouscritMesures/Dictionnaires/Technique/v1.0/ENEDIS.Dictionnaire.Technique.v1.0.xsd
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 08:40:19.598424 lowatt-enedis-2.2.1/lowatt_enedis/wsdl/CommandeArretServiceSouscritMesures/Services/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 08:40:19.622424 lowatt-enedis-2.2.1/lowatt_enedis/wsdl/CommandeArretServiceSouscritMesures/Services/CommandeArretServiceSouscritMesures/
+-rw-r--r--   0 runner    (1001) docker     (123)     3851 2023-06-19 08:40:11.000000 lowatt-enedis-2.2.1/lowatt_enedis/wsdl/CommandeArretServiceSouscritMesures/Services/CommandeArretServiceSouscritMesures/CommandeArretServiceSouscritMesures-v1.0.wsdl
+-rw-r--r--   0 runner    (1001) docker     (123)     2921 2023-06-19 08:40:11.000000 lowatt-enedis-2.2.1/lowatt_enedis/wsdl/CommandeArretServiceSouscritMesures/Services/CommandeArretServiceSouscritMesures/CommanderArretServiceSouscritMesures-v1.0.xsd
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 08:40:19.598424 lowatt-enedis-2.2.1/lowatt_enedis/wsdl/CommandeCollectePublicationMesures/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 08:40:19.598424 lowatt-enedis-2.2.1/lowatt_enedis/wsdl/CommandeCollectePublicationMesures/Dictionnaires/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 08:40:19.598424 lowatt-enedis-2.2.1/lowatt_enedis/wsdl/CommandeCollectePublicationMesures/Dictionnaires/Metier/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 08:40:19.622424 lowatt-enedis-2.2.1/lowatt_enedis/wsdl/CommandeCollectePublicationMesures/Dictionnaires/Metier/v5.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    36631 2023-06-19 08:40:11.000000 lowatt-enedis-2.2.1/lowatt_enedis/wsdl/CommandeCollectePublicationMesures/Dictionnaires/Metier/v5.0/ENEDIS.Dictionnaire.TypeComplexe.v5.0.xsd
+-rw-r--r--   0 runner    (1001) docker     (123)    37127 2023-06-19 08:40:11.000000 lowatt-enedis-2.2.1/lowatt_enedis/wsdl/CommandeCollectePublicationMesures/Dictionnaires/Metier/v5.0/ENEDIS.Dictionnaire.TypeSimple.v5.0.xsd
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 08:40:19.626424 lowatt-enedis-2.2.1/lowatt_enedis/wsdl/CommandeCollectePublicationMesures/Dictionnaires/Technique/
+-rw-r--r--   0 runner    (1001) docker     (123)     3201 2023-06-19 08:40:11.000000 lowatt-enedis-2.2.1/lowatt_enedis/wsdl/CommandeCollectePublicationMesures/Dictionnaires/Technique/W3C.SoapEnv.xsd
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 08:40:19.626424 lowatt-enedis-2.2.1/lowatt_enedis/wsdl/CommandeCollectePublicationMesures/Dictionnaires/Technique/v1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     4276 2023-06-19 08:40:11.000000 lowatt-enedis-2.2.1/lowatt_enedis/wsdl/CommandeCollectePublicationMesures/Dictionnaires/Technique/v1.0/ENEDIS.Dictionnaire.Technique.v1.0.xsd
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 08:40:19.598424 lowatt-enedis-2.2.1/lowatt_enedis/wsdl/CommandeCollectePublicationMesures/Services/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 08:40:19.626424 lowatt-enedis-2.2.1/lowatt_enedis/wsdl/CommandeCollectePublicationMesures/Services/CommandeCollectePublicationMesures/
+-rw-r--r--   0 runner    (1001) docker     (123)     3653 2023-06-19 08:40:11.000000 lowatt-enedis-2.2.1/lowatt_enedis/wsdl/CommandeCollectePublicationMesures/Services/CommandeCollectePublicationMesures/CommandeCollectePublicationMesures-v3.0.wsdl
+-rw-r--r--   0 runner    (1001) docker     (123)     4467 2023-06-19 08:40:11.000000 lowatt-enedis-2.2.1/lowatt_enedis/wsdl/CommandeCollectePublicationMesures/Services/CommandeCollectePublicationMesures/CommanderCollectePublicationMesures-v3.0.xsd
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 08:40:19.598424 lowatt-enedis-2.2.1/lowatt_enedis/wsdl/CommandeTransmissionDonneesInfraJ/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 08:40:19.598424 lowatt-enedis-2.2.1/lowatt_enedis/wsdl/CommandeTransmissionDonneesInfraJ/Dictionnaires/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 08:40:19.598424 lowatt-enedis-2.2.1/lowatt_enedis/wsdl/CommandeTransmissionDonneesInfraJ/Dictionnaires/Metier/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 08:40:19.630424 lowatt-enedis-2.2.1/lowatt_enedis/wsdl/CommandeTransmissionDonneesInfraJ/Dictionnaires/Metier/v5.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    37212 2023-06-19 08:40:11.000000 lowatt-enedis-2.2.1/lowatt_enedis/wsdl/CommandeTransmissionDonneesInfraJ/Dictionnaires/Metier/v5.0/ENEDIS.Dictionnaire.TypeComplexe.v5.0.xsd
+-rw-r--r--   0 runner    (1001) docker     (123)    38245 2023-06-19 08:40:11.000000 lowatt-enedis-2.2.1/lowatt_enedis/wsdl/CommandeTransmissionDonneesInfraJ/Dictionnaires/Metier/v5.0/ENEDIS.Dictionnaire.TypeSimple.v5.0.xsd
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 08:40:19.630424 lowatt-enedis-2.2.1/lowatt_enedis/wsdl/CommandeTransmissionDonneesInfraJ/Dictionnaires/Technique/
+-rw-r--r--   0 runner    (1001) docker     (123)     3201 2023-06-19 08:40:11.000000 lowatt-enedis-2.2.1/lowatt_enedis/wsdl/CommandeTransmissionDonneesInfraJ/Dictionnaires/Technique/W3C.SoapEnv.xsd
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 08:40:19.630424 lowatt-enedis-2.2.1/lowatt_enedis/wsdl/CommandeTransmissionDonneesInfraJ/Dictionnaires/Technique/v1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     4276 2023-06-19 08:40:11.000000 lowatt-enedis-2.2.1/lowatt_enedis/wsdl/CommandeTransmissionDonneesInfraJ/Dictionnaires/Technique/v1.0/ENEDIS.Dictionnaire.Technique.v1.0.xsd
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 08:40:19.598424 lowatt-enedis-2.2.1/lowatt_enedis/wsdl/CommandeTransmissionDonneesInfraJ/Services/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 08:40:19.630424 lowatt-enedis-2.2.1/lowatt_enedis/wsdl/CommandeTransmissionDonneesInfraJ/Services/CommandeTransmissionDonneesInfraJ/
+-rw-r--r--   0 runner    (1001) docker     (123)     3638 2023-06-19 08:40:11.000000 lowatt-enedis-2.2.1/lowatt_enedis/wsdl/CommandeTransmissionDonneesInfraJ/Services/CommandeTransmissionDonneesInfraJ/CommandeTransmissionDonneesInfraJ-v1.0.wsdl
+-rw-r--r--   0 runner    (1001) docker     (123)     4028 2023-06-19 08:40:11.000000 lowatt-enedis-2.2.1/lowatt_enedis/wsdl/CommandeTransmissionDonneesInfraJ/Services/CommandeTransmissionDonneesInfraJ/CommanderTransmissionDonneesInfraJ-v1.0.xsd
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 08:40:19.598424 lowatt-enedis-2.2.1/lowatt_enedis/wsdl/ConsultationDonneesTechniquesContractuelles/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 08:40:19.598424 lowatt-enedis-2.2.1/lowatt_enedis/wsdl/ConsultationDonneesTechniquesContractuelles/Dictionnaire/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 08:40:19.598424 lowatt-enedis-2.2.1/lowatt_enedis/wsdl/ConsultationDonneesTechniquesContractuelles/Dictionnaire/Metier/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 08:40:19.634424 lowatt-enedis-2.2.1/lowatt_enedis/wsdl/ConsultationDonneesTechniquesContractuelles/Dictionnaire/Metier/v5.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    37450 2023-06-19 08:40:11.000000 lowatt-enedis-2.2.1/lowatt_enedis/wsdl/ConsultationDonneesTechniquesContractuelles/Dictionnaire/Metier/v5.0/ENEDIS.Dictionnaire.TypeComplexe.v5.0.xsd
+-rw-r--r--   0 runner    (1001) docker     (123)    38416 2023-06-19 08:40:11.000000 lowatt-enedis-2.2.1/lowatt_enedis/wsdl/ConsultationDonneesTechniquesContractuelles/Dictionnaire/Metier/v5.0/ENEDIS.Dictionnaire.TypeSimple.v5.0.xsd
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 08:40:19.634424 lowatt-enedis-2.2.1/lowatt_enedis/wsdl/ConsultationDonneesTechniquesContractuelles/Dictionnaire/Technique/
+-rw-r--r--   0 runner    (1001) docker     (123)     4234 2023-06-19 08:40:11.000000 lowatt-enedis-2.2.1/lowatt_enedis/wsdl/ConsultationDonneesTechniquesContractuelles/Dictionnaire/Technique/ENEDIS.Dictionnaire.Technique.v1.0.xsd
+-rw-r--r--   0 runner    (1001) docker     (123)     6061 2023-06-19 08:40:11.000000 lowatt-enedis-2.2.1/lowatt_enedis/wsdl/ConsultationDonneesTechniquesContractuelles/Dictionnaire/Technique/W3C.SoapEnv.xsd
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 08:40:19.598424 lowatt-enedis-2.2.1/lowatt_enedis/wsdl/ConsultationDonneesTechniquesContractuelles/Services/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 08:40:19.634424 lowatt-enedis-2.2.1/lowatt_enedis/wsdl/ConsultationDonneesTechniquesContractuelles/Services/ConsultationDonneesTechniquesContractuelles/
+-rw-r--r--   0 runner    (1001) docker     (123)     3602 2023-06-19 08:40:11.000000 lowatt-enedis-2.2.1/lowatt_enedis/wsdl/ConsultationDonneesTechniquesContractuelles/Services/ConsultationDonneesTechniquesContractuelles/ConsultationDonneesTechniquesContractuelles-v1.0.wsdl
+-rw-r--r--   0 runner    (1001) docker     (123)    11723 2023-06-19 08:40:11.000000 lowatt-enedis-2.2.1/lowatt_enedis/wsdl/ConsultationDonneesTechniquesContractuelles/Services/ConsultationDonneesTechniquesContractuelles/ConsulterDonneesTechniquesContractuelles-v1.0.xsd
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 08:40:19.602424 lowatt-enedis-2.2.1/lowatt_enedis/wsdl/ConsultationMesures/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 08:40:19.602424 lowatt-enedis-2.2.1/lowatt_enedis/wsdl/ConsultationMesures/Dictionnaires/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 08:40:19.602424 lowatt-enedis-2.2.1/lowatt_enedis/wsdl/ConsultationMesures/Dictionnaires/Metier/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 08:40:19.634424 lowatt-enedis-2.2.1/lowatt_enedis/wsdl/ConsultationMesures/Dictionnaires/Metier/v5.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    37450 2023-06-19 08:40:11.000000 lowatt-enedis-2.2.1/lowatt_enedis/wsdl/ConsultationMesures/Dictionnaires/Metier/v5.0/ENEDIS.Dictionnaire.TypeComplexe.v5.0.xsd
+-rw-r--r--   0 runner    (1001) docker     (123)    38224 2023-06-19 08:40:11.000000 lowatt-enedis-2.2.1/lowatt_enedis/wsdl/ConsultationMesures/Dictionnaires/Metier/v5.0/ENEDIS.Dictionnaire.TypeSimple.v5.0.xsd
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 08:40:19.638424 lowatt-enedis-2.2.1/lowatt_enedis/wsdl/ConsultationMesures/Dictionnaires/Technique/
+-rw-r--r--   0 runner    (1001) docker     (123)     6061 2023-06-19 08:40:11.000000 lowatt-enedis-2.2.1/lowatt_enedis/wsdl/ConsultationMesures/Dictionnaires/Technique/W3C.SoapEnv.xsd
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 08:40:19.638424 lowatt-enedis-2.2.1/lowatt_enedis/wsdl/ConsultationMesures/Dictionnaires/Technique/v1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     4373 2023-06-19 08:40:11.000000 lowatt-enedis-2.2.1/lowatt_enedis/wsdl/ConsultationMesures/Dictionnaires/Technique/v1.0/ENEDIS.Dictionnaire.Technique.v1.0.xsd
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 08:40:19.602424 lowatt-enedis-2.2.1/lowatt_enedis/wsdl/ConsultationMesures/Services/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 08:40:19.638424 lowatt-enedis-2.2.1/lowatt_enedis/wsdl/ConsultationMesures/Services/ConsultationMesures/
+-rw-r--r--   0 runner    (1001) docker     (123)     2939 2023-06-19 08:40:11.000000 lowatt-enedis-2.2.1/lowatt_enedis/wsdl/ConsultationMesures/Services/ConsultationMesures/ConsultationMesures-v1.1.wsdl
+-rw-r--r--   0 runner    (1001) docker     (123)     3083 2023-06-19 08:40:11.000000 lowatt-enedis-2.2.1/lowatt_enedis/wsdl/ConsultationMesures/Services/ConsultationMesures/ConsulterMesures-v1.1.xsd
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 08:40:19.642424 lowatt-enedis-2.2.1/lowatt_enedis/wsdl/ConsultationMesuresDetaillees/
+-rw-r--r--   0 runner    (1001) docker     (123)     2652 2023-06-19 08:40:11.000000 lowatt-enedis-2.2.1/lowatt_enedis/wsdl/ConsultationMesuresDetaillees/ConsultationMesuresDetaillees-v2.0.wsdl
+-rw-r--r--   0 runner    (1001) docker     (123)     3793 2023-06-19 08:40:11.000000 lowatt-enedis-2.2.1/lowatt_enedis/wsdl/ConsultationMesuresDetaillees/ConsulterMesuresDetaillees-v2.0.1.xsd
+-rw-r--r--   0 runner    (1001) docker     (123)     4234 2023-06-19 08:40:11.000000 lowatt-enedis-2.2.1/lowatt_enedis/wsdl/ConsultationMesuresDetaillees/ENEDIS.Dictionnaire.Technique.v1.0.xsd
+-rw-r--r--   0 runner    (1001) docker     (123)     6177 2023-06-19 08:40:11.000000 lowatt-enedis-2.2.1/lowatt_enedis/wsdl/ConsultationMesuresDetaillees/W3C.SoapEnv.xsd
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 08:40:19.642424 lowatt-enedis-2.2.1/lowatt_enedis/wsdl/ConsultationMesuresDetailleesV3/
+-rw-r--r--   0 runner    (1001) docker     (123)    11126 2023-06-19 08:40:11.000000 lowatt-enedis-2.2.1/lowatt_enedis/wsdl/ConsultationMesuresDetailleesV3/ADAM.ConsulterMesuresDetailleesCommun.xsd
+-rw-r--r--   0 runner    (1001) docker     (123)     2977 2023-06-19 08:40:11.000000 lowatt-enedis-2.2.1/lowatt_enedis/wsdl/ConsultationMesuresDetailleesV3/ConsultationMesuresDetaillees-v3.0.wsdl
+-rw-r--r--   0 runner    (1001) docker     (123)     4835 2023-06-19 08:40:11.000000 lowatt-enedis-2.2.1/lowatt_enedis/wsdl/ConsultationMesuresDetailleesV3/ENEDIS.Dictionnaire.Technique.v1.0.xsd
+-rw-r--r--   0 runner    (1001) docker     (123)     6426 2023-06-19 08:40:11.000000 lowatt-enedis-2.2.1/lowatt_enedis/wsdl/ConsultationMesuresDetailleesV3/W3C.SoapEnv.xsd
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 08:40:19.602424 lowatt-enedis-2.2.1/lowatt_enedis/wsdl/RecherchePoint/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 08:40:19.602424 lowatt-enedis-2.2.1/lowatt_enedis/wsdl/RecherchePoint/Dictionnaires/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 08:40:19.646424 lowatt-enedis-2.2.1/lowatt_enedis/wsdl/RecherchePoint/Dictionnaires/Technique/
+-rw-r--r--   0 runner    (1001) docker     (123)     4328 2023-06-19 08:40:11.000000 lowatt-enedis-2.2.1/lowatt_enedis/wsdl/RecherchePoint/Dictionnaires/Technique/ENEDIS.Dictionnaire.Technique.v1.0.xsd
+-rw-r--r--   0 runner    (1001) docker     (123)     6177 2023-06-19 08:40:11.000000 lowatt-enedis-2.2.1/lowatt_enedis/wsdl/RecherchePoint/Dictionnaires/Technique/W3C.SoapEnv.xsd
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 08:40:19.646424 lowatt-enedis-2.2.1/lowatt_enedis/wsdl/RecherchePoint/Dictionnaires/v5.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    37450 2023-06-19 08:40:11.000000 lowatt-enedis-2.2.1/lowatt_enedis/wsdl/RecherchePoint/Dictionnaires/v5.0/ENEDIS.Dictionnaire.TypeComplexe.v5.0.xsd
+-rw-r--r--   0 runner    (1001) docker     (123)    38452 2023-06-19 08:40:11.000000 lowatt-enedis-2.2.1/lowatt_enedis/wsdl/RecherchePoint/Dictionnaires/v5.0/ENEDIS.Dictionnaire.TypeSimple.v5.0.xsd
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 08:40:19.602424 lowatt-enedis-2.2.1/lowatt_enedis/wsdl/RecherchePoint/Services/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 08:40:19.646424 lowatt-enedis-2.2.1/lowatt_enedis/wsdl/RecherchePoint/Services/RecherchePoint/
+-rw-r--r--   0 runner    (1001) docker     (123)     2872 2023-06-19 08:40:11.000000 lowatt-enedis-2.2.1/lowatt_enedis/wsdl/RecherchePoint/Services/RecherchePoint/RecherchePoint-v2.0.wsdl
+-rw-r--r--   0 runner    (1001) docker     (123)     3467 2023-06-19 08:40:11.000000 lowatt-enedis-2.2.1/lowatt_enedis/wsdl/RecherchePoint/Services/RecherchePoint/RechercherPoint-v2.0.xsd
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 08:40:19.602424 lowatt-enedis-2.2.1/lowatt_enedis/wsdl/RechercheServicesSouscritsMesures/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 08:40:19.602424 lowatt-enedis-2.2.1/lowatt_enedis/wsdl/RechercheServicesSouscritsMesures/Dictionnaires/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 08:40:19.602424 lowatt-enedis-2.2.1/lowatt_enedis/wsdl/RechercheServicesSouscritsMesures/Dictionnaires/Metier/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 08:40:19.650425 lowatt-enedis-2.2.1/lowatt_enedis/wsdl/RechercheServicesSouscritsMesures/Dictionnaires/Metier/v5.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    37212 2023-06-19 08:40:11.000000 lowatt-enedis-2.2.1/lowatt_enedis/wsdl/RechercheServicesSouscritsMesures/Dictionnaires/Metier/v5.0/ENEDIS.Dictionnaire.TypeComplexe.v5.0.xsd
+-rw-r--r--   0 runner    (1001) docker     (123)    38245 2023-06-19 08:40:11.000000 lowatt-enedis-2.2.1/lowatt_enedis/wsdl/RechercheServicesSouscritsMesures/Dictionnaires/Metier/v5.0/ENEDIS.Dictionnaire.TypeSimple.v5.0.xsd
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 08:40:19.650425 lowatt-enedis-2.2.1/lowatt_enedis/wsdl/RechercheServicesSouscritsMesures/Dictionnaires/Technique/
+-rw-r--r--   0 runner    (1001) docker     (123)     3062 2023-06-19 08:40:11.000000 lowatt-enedis-2.2.1/lowatt_enedis/wsdl/RechercheServicesSouscritsMesures/Dictionnaires/Technique/W3C.SoapEnv.xsd
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 08:40:19.650425 lowatt-enedis-2.2.1/lowatt_enedis/wsdl/RechercheServicesSouscritsMesures/Dictionnaires/Technique/v1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     4025 2023-06-19 08:40:11.000000 lowatt-enedis-2.2.1/lowatt_enedis/wsdl/RechercheServicesSouscritsMesures/Dictionnaires/Technique/v1.0/ENEDIS.Dictionnaire.Technique.v1.0.xsd
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 08:40:19.602424 lowatt-enedis-2.2.1/lowatt_enedis/wsdl/RechercheServicesSouscritsMesures/Services/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 08:40:19.650425 lowatt-enedis-2.2.1/lowatt_enedis/wsdl/RechercheServicesSouscritsMesures/Services/RechercheServicesSouscritsMesures/
+-rw-r--r--   0 runner    (1001) docker     (123)     3321 2023-06-19 08:40:11.000000 lowatt-enedis-2.2.1/lowatt_enedis/wsdl/RechercheServicesSouscritsMesures/Services/RechercheServicesSouscritsMesures/RechercherServicesSouscritsMesures-v1.0.wsdl
+-rw-r--r--   0 runner    (1001) docker     (123)     3423 2023-06-19 08:40:11.000000 lowatt-enedis-2.2.1/lowatt_enedis/wsdl/RechercheServicesSouscritsMesures/Services/RechercheServicesSouscritsMesures/RechercherServicesSouscritsMesures-v1.0.xsd
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 08:40:19.602424 lowatt-enedis-2.2.1/lowatt_enedis/wsdl/TransmissionHistoriqueMesures/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 08:40:19.602424 lowatt-enedis-2.2.1/lowatt_enedis/wsdl/TransmissionHistoriqueMesures/Dictionnaires/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 08:40:19.654425 lowatt-enedis-2.2.1/lowatt_enedis/wsdl/TransmissionHistoriqueMesures/Dictionnaires/v4.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    40590 2023-06-19 08:40:11.000000 lowatt-enedis-2.2.1/lowatt_enedis/wsdl/TransmissionHistoriqueMesures/Dictionnaires/v4.0/ERDF.Dictionnaire.TypeComplexe.v4.0.xsd
+-rw-r--r--   0 runner    (1001) docker     (123)    36163 2023-06-19 08:40:11.000000 lowatt-enedis-2.2.1/lowatt_enedis/wsdl/TransmissionHistoriqueMesures/Dictionnaires/v4.0/ERDF.Dictionnaire.TypeSimple.v4.0.xsd
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 08:40:19.602424 lowatt-enedis-2.2.1/lowatt_enedis/wsdl/TransmissionHistoriqueMesures/Services/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 08:40:19.654425 lowatt-enedis-2.2.1/lowatt_enedis/wsdl/TransmissionHistoriqueMesures/Services/TransmissionHistoriqueMesures/
+-rw-r--r--   0 runner    (1001) docker     (123)     3514 2023-06-19 08:40:11.000000 lowatt-enedis-2.2.1/lowatt_enedis/wsdl/TransmissionHistoriqueMesures/Services/TransmissionHistoriqueMesures/CommandeTransmissionHistoriqueMesures-v1.0.wsdl
+-rw-r--r--   0 runner    (1001) docker     (123)     4704 2023-06-19 08:40:11.000000 lowatt-enedis-2.2.1/lowatt_enedis/wsdl/TransmissionHistoriqueMesures/Services/TransmissionHistoriqueMesures/CommanderTransmissionHistoriqueMesures-v1.0.xsd
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 08:40:19.614424 lowatt-enedis-2.2.1/lowatt_enedis.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3030 2023-06-19 08:40:19.000000 lowatt-enedis-2.2.1/lowatt_enedis.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7414 2023-06-19 08:40:19.000000 lowatt-enedis-2.2.1/lowatt_enedis.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-19 08:40:19.000000 lowatt-enedis-2.2.1/lowatt_enedis.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-06-19 08:40:19.000000 lowatt-enedis-2.2.1/lowatt_enedis.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      164 2023-06-19 08:40:19.000000 lowatt-enedis-2.2.1/lowatt_enedis.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-19 08:40:19.000000 lowatt-enedis-2.2.1/lowatt_enedis.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      227 2023-06-19 08:40:11.000000 lowatt-enedis-2.2.1/mypy.ini
+-rw-r--r--   0 runner    (1001) docker     (123)      242 2023-06-19 08:40:11.000000 lowatt-enedis-2.2.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-06-19 08:40:11.000000 lowatt-enedis-2.2.1/pytest.ini
+-rw-r--r--   0 runner    (1001) docker     (123)     1004 2023-06-19 08:40:19.666425 lowatt-enedis-2.2.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      669 2023-06-19 08:40:11.000000 lowatt-enedis-2.2.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 08:40:19.658424 lowatt-enedis-2.2.1/test/
+-rw-r--r--   0 runner    (1001) docker     (123)      421 2023-06-19 08:40:11.000000 lowatt-enedis-2.2.1/test/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 08:40:19.658424 lowatt-enedis-2.2.1/test/data/
+-rw-r--r--   0 runner    (1001) docker     (123)     1319 2023-06-19 08:40:11.000000 lowatt-enedis-2.2.1/test/data/consulterMesuresDetailleesResponse.xml
+-rw-r--r--   0 runner    (1001) docker     (123)     4247 2023-06-19 08:40:11.000000 lowatt-enedis-2.2.1/test/data/consulterMesuresResponse.xml
+-rw-r--r--   0 runner    (1001) docker     (123)    92977 2023-06-19 08:40:11.000000 lowatt-enedis-2.2.1/test/data/requests.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     5804 2023-06-19 08:40:11.000000 lowatt-enedis-2.2.1/test/test_lowatt_enedis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4863 2023-06-19 08:40:11.000000 lowatt-enedis-2.2.1/test/test_requests.py
+-rw-r--r--   0 runner    (1001) docker     (123)      815 2023-06-19 08:40:11.000000 lowatt-enedis-2.2.1/tox.ini
```

### Comparing `lowatt-enedis-2.2.0/.flake8` & `lowatt-enedis-2.2.1/.flake8`

 * *Files identical despite different names*

### Comparing `lowatt-enedis-2.2.0/.github/workflows/tox.yml` & `lowatt-enedis-2.2.1/.github/workflows/tox.yml`

 * *Files identical despite different names*

### Comparing `lowatt-enedis-2.2.0/COPYING` & `lowatt-enedis-2.2.1/COPYING`

 * *Files identical despite different names*

### Comparing `lowatt-enedis-2.2.0/PKG-INFO` & `lowatt-enedis-2.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lowatt-enedis
-Version: 2.2.0
+Version: 2.2.1
 Summary: Query Enedis SGE web-service
 Home-page: https://github.com/lowatt/lowatt-enedis
 Author: Lowatt
 Author-email: info@lowatt.fr
 License: GPL3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `lowatt-enedis-2.2.0/README.md` & `lowatt-enedis-2.2.1/README.md`

 * *Files identical despite different names*

### Comparing `lowatt-enedis-2.2.0/lowatt_enedis/__init__.py` & `lowatt-enedis-2.2.1/lowatt_enedis/__init__.py`

 * *Files identical despite different names*

### Comparing `lowatt-enedis-2.2.0/lowatt_enedis/__main__.py` & `lowatt-enedis-2.2.1/lowatt_enedis/__main__.py`

 * *Files identical despite different names*

### Comparing `lowatt-enedis-2.2.0/lowatt_enedis/certauth.py` & `lowatt-enedis-2.2.1/lowatt_enedis/certauth.py`

 * *Files 5% similar despite different names*

```diff
@@ -28,29 +28,31 @@
 """
 
 import ssl
 from http.client import HTTPResponse, HTTPSConnection
 from typing import Any
 from urllib.request import HTTPSHandler, Request, build_opener
 
+import certifi
 from suds.transport.http import HttpTransport
 
 
 class _HTTPSClientAuthHandler(HTTPSHandler):
     def __init__(self, cert_file: str, key_file: str):
         super().__init__()
         self.cert_file = cert_file
         self.key_file = key_file
 
     def https_open(self, req: Request) -> HTTPResponse:
         return self.do_open(self.get_connection, req)  # type: ignore[arg-type]
 
     def get_connection(self, host: str, timeout: int = 300) -> HTTPSConnection:
-        context = ssl.SSLContext()
+        context = ssl.SSLContext(protocol=ssl.PROTOCOL_TLS_CLIENT)
         context.load_cert_chain(self.cert_file, self.key_file)
+        context.load_verify_locations(cafile=certifi.where())
         return HTTPSConnection(host, context=context)
 
 
 class HTTPSClientCertTransport(HttpTransport):  # type: ignore[misc]
     """SUDS_ transport class to connect through an HTTPS connection using
     a client SSL certificate.
```

### Comparing `lowatt-enedis-2.2.0/lowatt_enedis/services.py` & `lowatt-enedis-2.2.1/lowatt_enedis/services.py`

 * *Files identical despite different names*

### Comparing `lowatt-enedis-2.2.0/lowatt_enedis/wsdl/CommandeAccesDonneesMesures/Services/CommanderAccesDonneesMesures/CommanderAccesDonneesMesures-V1.0.wsdl` & `lowatt-enedis-2.2.1/lowatt_enedis/wsdl/CommandeAccesDonneesMesures/Services/CommanderAccesDonneesMesures/CommanderAccesDonneesMesures-V1.0.wsdl`

 * *Files identical despite different names*

### Comparing `lowatt-enedis-2.2.0/lowatt_enedis/wsdl/CommandeAccesDonneesMesures/Services/CommanderAccesDonneesMesures/CommanderAccesDonneesMesures-V1.0.xsd` & `lowatt-enedis-2.2.1/lowatt_enedis/wsdl/CommandeAccesDonneesMesures/Services/CommanderAccesDonneesMesures/CommanderAccesDonneesMesures-V1.0.xsd`

 * *Files identical despite different names*

### Comparing `lowatt-enedis-2.2.0/lowatt_enedis/wsdl/CommandeAccesDonneesMesures/Services/CommanderAccesDonneesMesures/ENEDIS.Dictionnaire.Technique.v1.0.xsd` & `lowatt-enedis-2.2.1/lowatt_enedis/wsdl/CommandeAccesDonneesMesures/Services/CommanderAccesDonneesMesures/ENEDIS.Dictionnaire.Technique.v1.0.xsd`

 * *Files identical despite different names*

### Comparing `lowatt-enedis-2.2.0/lowatt_enedis/wsdl/CommandeAccesDonneesMesures/Services/CommanderAccesDonneesMesures/ENEDIS.Dictionnaire.TypeComplexe.v5.0.xsd` & `lowatt-enedis-2.2.1/lowatt_enedis/wsdl/CommandeAccesDonneesMesures/Services/CommanderAccesDonneesMesures/ENEDIS.Dictionnaire.TypeComplexe.v5.0.xsd`

 * *Files identical despite different names*

### Comparing `lowatt-enedis-2.2.0/lowatt_enedis/wsdl/CommandeAccesDonneesMesures/Services/CommanderAccesDonneesMesures/ENEDIS.Dictionnaire.TypeSimple.v5.0.xsd` & `lowatt-enedis-2.2.1/lowatt_enedis/wsdl/CommandeAccesDonneesMesures/Services/CommanderAccesDonneesMesures/ENEDIS.Dictionnaire.TypeSimple.v5.0.xsd`

 * *Files identical despite different names*

### Comparing `lowatt-enedis-2.2.0/lowatt_enedis/wsdl/CommandeAccesDonneesMesures/Services/CommanderAccesDonneesMesures/W3C.SoapEnv.xsd` & `lowatt-enedis-2.2.1/lowatt_enedis/wsdl/CommandeAccesDonneesMesures/Services/CommanderAccesDonneesMesures/W3C.SoapEnv.xsd`

 * *Files identical despite different names*

### Comparing `lowatt-enedis-2.2.0/lowatt_enedis/wsdl/CommandeArretServiceSouscritMesures/Dictionnaires/Metier/v5.0/ENEDIS.Dictionnaire.TypeComplexe.v5.0.xsd` & `lowatt-enedis-2.2.1/lowatt_enedis/wsdl/CommandeArretServiceSouscritMesures/Dictionnaires/Metier/v5.0/ENEDIS.Dictionnaire.TypeComplexe.v5.0.xsd`

 * *Files identical despite different names*

### Comparing `lowatt-enedis-2.2.0/lowatt_enedis/wsdl/CommandeArretServiceSouscritMesures/Dictionnaires/Metier/v5.0/ENEDIS.Dictionnaire.TypeSimple.v5.0.xsd` & `lowatt-enedis-2.2.1/lowatt_enedis/wsdl/CommandeArretServiceSouscritMesures/Dictionnaires/Metier/v5.0/ENEDIS.Dictionnaire.TypeSimple.v5.0.xsd`

 * *Files identical despite different names*

### Comparing `lowatt-enedis-2.2.0/lowatt_enedis/wsdl/CommandeArretServiceSouscritMesures/Dictionnaires/Technique/W3C.SoapEnv.xsd` & `lowatt-enedis-2.2.1/lowatt_enedis/wsdl/CommandeArretServiceSouscritMesures/Dictionnaires/Technique/W3C.SoapEnv.xsd`

 * *Files identical despite different names*

### Comparing `lowatt-enedis-2.2.0/lowatt_enedis/wsdl/CommandeArretServiceSouscritMesures/Dictionnaires/Technique/v1.0/ENEDIS.Dictionnaire.Technique.v1.0.xsd` & `lowatt-enedis-2.2.1/lowatt_enedis/wsdl/CommandeArretServiceSouscritMesures/Dictionnaires/Technique/v1.0/ENEDIS.Dictionnaire.Technique.v1.0.xsd`

 * *Files identical despite different names*

### Comparing `lowatt-enedis-2.2.0/lowatt_enedis/wsdl/CommandeArretServiceSouscritMesures/Services/CommandeArretServiceSouscritMesures/CommandeArretServiceSouscritMesures-v1.0.wsdl` & `lowatt-enedis-2.2.1/lowatt_enedis/wsdl/CommandeArretServiceSouscritMesures/Services/CommandeArretServiceSouscritMesures/CommandeArretServiceSouscritMesures-v1.0.wsdl`

 * *Files identical despite different names*

### Comparing `lowatt-enedis-2.2.0/lowatt_enedis/wsdl/CommandeArretServiceSouscritMesures/Services/CommandeArretServiceSouscritMesures/CommanderArretServiceSouscritMesures-v1.0.xsd` & `lowatt-enedis-2.2.1/lowatt_enedis/wsdl/CommandeArretServiceSouscritMesures/Services/CommandeArretServiceSouscritMesures/CommanderArretServiceSouscritMesures-v1.0.xsd`

 * *Files identical despite different names*

### Comparing `lowatt-enedis-2.2.0/lowatt_enedis/wsdl/CommandeCollectePublicationMesures/Dictionnaires/Metier/v5.0/ENEDIS.Dictionnaire.TypeComplexe.v5.0.xsd` & `lowatt-enedis-2.2.1/lowatt_enedis/wsdl/CommandeCollectePublicationMesures/Dictionnaires/Metier/v5.0/ENEDIS.Dictionnaire.TypeComplexe.v5.0.xsd`

 * *Files identical despite different names*

### Comparing `lowatt-enedis-2.2.0/lowatt_enedis/wsdl/CommandeCollectePublicationMesures/Dictionnaires/Metier/v5.0/ENEDIS.Dictionnaire.TypeSimple.v5.0.xsd` & `lowatt-enedis-2.2.1/lowatt_enedis/wsdl/CommandeCollectePublicationMesures/Dictionnaires/Metier/v5.0/ENEDIS.Dictionnaire.TypeSimple.v5.0.xsd`

 * *Files identical despite different names*

### Comparing `lowatt-enedis-2.2.0/lowatt_enedis/wsdl/CommandeCollectePublicationMesures/Dictionnaires/Technique/W3C.SoapEnv.xsd` & `lowatt-enedis-2.2.1/lowatt_enedis/wsdl/CommandeCollectePublicationMesures/Dictionnaires/Technique/W3C.SoapEnv.xsd`

 * *Files identical despite different names*

### Comparing `lowatt-enedis-2.2.0/lowatt_enedis/wsdl/CommandeCollectePublicationMesures/Dictionnaires/Technique/v1.0/ENEDIS.Dictionnaire.Technique.v1.0.xsd` & `lowatt-enedis-2.2.1/lowatt_enedis/wsdl/CommandeCollectePublicationMesures/Dictionnaires/Technique/v1.0/ENEDIS.Dictionnaire.Technique.v1.0.xsd`

 * *Files identical despite different names*

### Comparing `lowatt-enedis-2.2.0/lowatt_enedis/wsdl/CommandeCollectePublicationMesures/Services/CommandeCollectePublicationMesures/CommandeCollectePublicationMesures-v3.0.wsdl` & `lowatt-enedis-2.2.1/lowatt_enedis/wsdl/CommandeCollectePublicationMesures/Services/CommandeCollectePublicationMesures/CommandeCollectePublicationMesures-v3.0.wsdl`

 * *Files identical despite different names*

### Comparing `lowatt-enedis-2.2.0/lowatt_enedis/wsdl/CommandeCollectePublicationMesures/Services/CommandeCollectePublicationMesures/CommanderCollectePublicationMesures-v3.0.xsd` & `lowatt-enedis-2.2.1/lowatt_enedis/wsdl/CommandeCollectePublicationMesures/Services/CommandeCollectePublicationMesures/CommanderCollectePublicationMesures-v3.0.xsd`

 * *Files identical despite different names*

### Comparing `lowatt-enedis-2.2.0/lowatt_enedis/wsdl/CommandeTransmissionDonneesInfraJ/Dictionnaires/Metier/v5.0/ENEDIS.Dictionnaire.TypeComplexe.v5.0.xsd` & `lowatt-enedis-2.2.1/lowatt_enedis/wsdl/CommandeTransmissionDonneesInfraJ/Dictionnaires/Metier/v5.0/ENEDIS.Dictionnaire.TypeComplexe.v5.0.xsd`

 * *Files identical despite different names*

### Comparing `lowatt-enedis-2.2.0/lowatt_enedis/wsdl/CommandeTransmissionDonneesInfraJ/Dictionnaires/Metier/v5.0/ENEDIS.Dictionnaire.TypeSimple.v5.0.xsd` & `lowatt-enedis-2.2.1/lowatt_enedis/wsdl/CommandeTransmissionDonneesInfraJ/Dictionnaires/Metier/v5.0/ENEDIS.Dictionnaire.TypeSimple.v5.0.xsd`

 * *Files identical despite different names*

### Comparing `lowatt-enedis-2.2.0/lowatt_enedis/wsdl/CommandeTransmissionDonneesInfraJ/Dictionnaires/Technique/W3C.SoapEnv.xsd` & `lowatt-enedis-2.2.1/lowatt_enedis/wsdl/CommandeTransmissionDonneesInfraJ/Dictionnaires/Technique/W3C.SoapEnv.xsd`

 * *Files identical despite different names*

### Comparing `lowatt-enedis-2.2.0/lowatt_enedis/wsdl/CommandeTransmissionDonneesInfraJ/Dictionnaires/Technique/v1.0/ENEDIS.Dictionnaire.Technique.v1.0.xsd` & `lowatt-enedis-2.2.1/lowatt_enedis/wsdl/CommandeTransmissionDonneesInfraJ/Dictionnaires/Technique/v1.0/ENEDIS.Dictionnaire.Technique.v1.0.xsd`

 * *Files identical despite different names*

### Comparing `lowatt-enedis-2.2.0/lowatt_enedis/wsdl/CommandeTransmissionDonneesInfraJ/Services/CommandeTransmissionDonneesInfraJ/CommandeTransmissionDonneesInfraJ-v1.0.wsdl` & `lowatt-enedis-2.2.1/lowatt_enedis/wsdl/CommandeTransmissionDonneesInfraJ/Services/CommandeTransmissionDonneesInfraJ/CommandeTransmissionDonneesInfraJ-v1.0.wsdl`

 * *Files identical despite different names*

### Comparing `lowatt-enedis-2.2.0/lowatt_enedis/wsdl/CommandeTransmissionDonneesInfraJ/Services/CommandeTransmissionDonneesInfraJ/CommanderTransmissionDonneesInfraJ-v1.0.xsd` & `lowatt-enedis-2.2.1/lowatt_enedis/wsdl/CommandeTransmissionDonneesInfraJ/Services/CommandeTransmissionDonneesInfraJ/CommanderTransmissionDonneesInfraJ-v1.0.xsd`

 * *Files identical despite different names*

### Comparing `lowatt-enedis-2.2.0/lowatt_enedis/wsdl/ConsultationDonneesTechniquesContractuelles/Dictionnaire/Metier/v5.0/ENEDIS.Dictionnaire.TypeComplexe.v5.0.xsd` & `lowatt-enedis-2.2.1/lowatt_enedis/wsdl/ConsultationDonneesTechniquesContractuelles/Dictionnaire/Metier/v5.0/ENEDIS.Dictionnaire.TypeComplexe.v5.0.xsd`

 * *Files identical despite different names*

### Comparing `lowatt-enedis-2.2.0/lowatt_enedis/wsdl/ConsultationDonneesTechniquesContractuelles/Dictionnaire/Metier/v5.0/ENEDIS.Dictionnaire.TypeSimple.v5.0.xsd` & `lowatt-enedis-2.2.1/lowatt_enedis/wsdl/ConsultationDonneesTechniquesContractuelles/Dictionnaire/Metier/v5.0/ENEDIS.Dictionnaire.TypeSimple.v5.0.xsd`

 * *Files identical despite different names*

### Comparing `lowatt-enedis-2.2.0/lowatt_enedis/wsdl/ConsultationDonneesTechniquesContractuelles/Dictionnaire/Technique/ENEDIS.Dictionnaire.Technique.v1.0.xsd` & `lowatt-enedis-2.2.1/lowatt_enedis/wsdl/ConsultationDonneesTechniquesContractuelles/Dictionnaire/Technique/ENEDIS.Dictionnaire.Technique.v1.0.xsd`

 * *Files identical despite different names*

### Comparing `lowatt-enedis-2.2.0/lowatt_enedis/wsdl/ConsultationDonneesTechniquesContractuelles/Dictionnaire/Technique/W3C.SoapEnv.xsd` & `lowatt-enedis-2.2.1/lowatt_enedis/wsdl/ConsultationDonneesTechniquesContractuelles/Dictionnaire/Technique/W3C.SoapEnv.xsd`

 * *Files identical despite different names*

### Comparing `lowatt-enedis-2.2.0/lowatt_enedis/wsdl/ConsultationDonneesTechniquesContractuelles/Services/ConsultationDonneesTechniquesContractuelles/ConsultationDonneesTechniquesContractuelles-v1.0.wsdl` & `lowatt-enedis-2.2.1/lowatt_enedis/wsdl/ConsultationDonneesTechniquesContractuelles/Services/ConsultationDonneesTechniquesContractuelles/ConsultationDonneesTechniquesContractuelles-v1.0.wsdl`

 * *Files identical despite different names*

### Comparing `lowatt-enedis-2.2.0/lowatt_enedis/wsdl/ConsultationDonneesTechniquesContractuelles/Services/ConsultationDonneesTechniquesContractuelles/ConsulterDonneesTechniquesContractuelles-v1.0.xsd` & `lowatt-enedis-2.2.1/lowatt_enedis/wsdl/ConsultationDonneesTechniquesContractuelles/Services/ConsultationDonneesTechniquesContractuelles/ConsulterDonneesTechniquesContractuelles-v1.0.xsd`

 * *Files identical despite different names*

### Comparing `lowatt-enedis-2.2.0/lowatt_enedis/wsdl/ConsultationMesures/Dictionnaires/Metier/v5.0/ENEDIS.Dictionnaire.TypeComplexe.v5.0.xsd` & `lowatt-enedis-2.2.1/lowatt_enedis/wsdl/ConsultationMesures/Dictionnaires/Metier/v5.0/ENEDIS.Dictionnaire.TypeComplexe.v5.0.xsd`

 * *Files identical despite different names*

### Comparing `lowatt-enedis-2.2.0/lowatt_enedis/wsdl/ConsultationMesures/Dictionnaires/Metier/v5.0/ENEDIS.Dictionnaire.TypeSimple.v5.0.xsd` & `lowatt-enedis-2.2.1/lowatt_enedis/wsdl/ConsultationMesures/Dictionnaires/Metier/v5.0/ENEDIS.Dictionnaire.TypeSimple.v5.0.xsd`

 * *Files identical despite different names*

### Comparing `lowatt-enedis-2.2.0/lowatt_enedis/wsdl/ConsultationMesures/Dictionnaires/Technique/W3C.SoapEnv.xsd` & `lowatt-enedis-2.2.1/lowatt_enedis/wsdl/ConsultationMesures/Dictionnaires/Technique/W3C.SoapEnv.xsd`

 * *Files identical despite different names*

### Comparing `lowatt-enedis-2.2.0/lowatt_enedis/wsdl/ConsultationMesures/Dictionnaires/Technique/v1.0/ENEDIS.Dictionnaire.Technique.v1.0.xsd` & `lowatt-enedis-2.2.1/lowatt_enedis/wsdl/ConsultationMesures/Dictionnaires/Technique/v1.0/ENEDIS.Dictionnaire.Technique.v1.0.xsd`

 * *Files identical despite different names*

### Comparing `lowatt-enedis-2.2.0/lowatt_enedis/wsdl/ConsultationMesures/Services/ConsultationMesures/ConsultationMesures-v1.1.wsdl` & `lowatt-enedis-2.2.1/lowatt_enedis/wsdl/ConsultationMesures/Services/ConsultationMesures/ConsultationMesures-v1.1.wsdl`

 * *Files identical despite different names*

### Comparing `lowatt-enedis-2.2.0/lowatt_enedis/wsdl/ConsultationMesures/Services/ConsultationMesures/ConsulterMesures-v1.1.xsd` & `lowatt-enedis-2.2.1/lowatt_enedis/wsdl/ConsultationMesures/Services/ConsultationMesures/ConsulterMesures-v1.1.xsd`

 * *Files identical despite different names*

### Comparing `lowatt-enedis-2.2.0/lowatt_enedis/wsdl/ConsultationMesuresDetaillees/ConsultationMesuresDetaillees-v2.0.wsdl` & `lowatt-enedis-2.2.1/lowatt_enedis/wsdl/ConsultationMesuresDetaillees/ConsultationMesuresDetaillees-v2.0.wsdl`

 * *Files identical despite different names*

### Comparing `lowatt-enedis-2.2.0/lowatt_enedis/wsdl/ConsultationMesuresDetaillees/ConsulterMesuresDetaillees-v2.0.1.xsd` & `lowatt-enedis-2.2.1/lowatt_enedis/wsdl/ConsultationMesuresDetaillees/ConsulterMesuresDetaillees-v2.0.1.xsd`

 * *Files identical despite different names*

### Comparing `lowatt-enedis-2.2.0/lowatt_enedis/wsdl/ConsultationMesuresDetaillees/ENEDIS.Dictionnaire.Technique.v1.0.xsd` & `lowatt-enedis-2.2.1/lowatt_enedis/wsdl/ConsultationMesuresDetaillees/ENEDIS.Dictionnaire.Technique.v1.0.xsd`

 * *Files identical despite different names*

### Comparing `lowatt-enedis-2.2.0/lowatt_enedis/wsdl/ConsultationMesuresDetaillees/W3C.SoapEnv.xsd` & `lowatt-enedis-2.2.1/lowatt_enedis/wsdl/ConsultationMesuresDetaillees/W3C.SoapEnv.xsd`

 * *Files identical despite different names*

### Comparing `lowatt-enedis-2.2.0/lowatt_enedis/wsdl/ConsultationMesuresDetailleesV3/ADAM.ConsulterMesuresDetailleesCommun.xsd` & `lowatt-enedis-2.2.1/lowatt_enedis/wsdl/ConsultationMesuresDetailleesV3/ADAM.ConsulterMesuresDetailleesCommun.xsd`

 * *Files identical despite different names*

### Comparing `lowatt-enedis-2.2.0/lowatt_enedis/wsdl/ConsultationMesuresDetailleesV3/ConsultationMesuresDetaillees-v3.0.wsdl` & `lowatt-enedis-2.2.1/lowatt_enedis/wsdl/ConsultationMesuresDetailleesV3/ConsultationMesuresDetaillees-v3.0.wsdl`

 * *Files identical despite different names*

### Comparing `lowatt-enedis-2.2.0/lowatt_enedis/wsdl/ConsultationMesuresDetailleesV3/ENEDIS.Dictionnaire.Technique.v1.0.xsd` & `lowatt-enedis-2.2.1/lowatt_enedis/wsdl/ConsultationMesuresDetailleesV3/ENEDIS.Dictionnaire.Technique.v1.0.xsd`

 * *Files identical despite different names*

### Comparing `lowatt-enedis-2.2.0/lowatt_enedis/wsdl/ConsultationMesuresDetailleesV3/W3C.SoapEnv.xsd` & `lowatt-enedis-2.2.1/lowatt_enedis/wsdl/ConsultationMesuresDetailleesV3/W3C.SoapEnv.xsd`

 * *Files identical despite different names*

### Comparing `lowatt-enedis-2.2.0/lowatt_enedis/wsdl/RecherchePoint/Dictionnaires/Technique/ENEDIS.Dictionnaire.Technique.v1.0.xsd` & `lowatt-enedis-2.2.1/lowatt_enedis/wsdl/RecherchePoint/Dictionnaires/Technique/ENEDIS.Dictionnaire.Technique.v1.0.xsd`

 * *Files identical despite different names*

### Comparing `lowatt-enedis-2.2.0/lowatt_enedis/wsdl/RecherchePoint/Dictionnaires/Technique/W3C.SoapEnv.xsd` & `lowatt-enedis-2.2.1/lowatt_enedis/wsdl/RecherchePoint/Dictionnaires/Technique/W3C.SoapEnv.xsd`

 * *Files identical despite different names*

### Comparing `lowatt-enedis-2.2.0/lowatt_enedis/wsdl/RecherchePoint/Dictionnaires/v5.0/ENEDIS.Dictionnaire.TypeComplexe.v5.0.xsd` & `lowatt-enedis-2.2.1/lowatt_enedis/wsdl/RecherchePoint/Dictionnaires/v5.0/ENEDIS.Dictionnaire.TypeComplexe.v5.0.xsd`

 * *Files identical despite different names*

### Comparing `lowatt-enedis-2.2.0/lowatt_enedis/wsdl/RecherchePoint/Dictionnaires/v5.0/ENEDIS.Dictionnaire.TypeSimple.v5.0.xsd` & `lowatt-enedis-2.2.1/lowatt_enedis/wsdl/RecherchePoint/Dictionnaires/v5.0/ENEDIS.Dictionnaire.TypeSimple.v5.0.xsd`

 * *Files identical despite different names*

### Comparing `lowatt-enedis-2.2.0/lowatt_enedis/wsdl/RecherchePoint/Services/RecherchePoint/RecherchePoint-v2.0.wsdl` & `lowatt-enedis-2.2.1/lowatt_enedis/wsdl/RecherchePoint/Services/RecherchePoint/RecherchePoint-v2.0.wsdl`

 * *Files identical despite different names*

### Comparing `lowatt-enedis-2.2.0/lowatt_enedis/wsdl/RecherchePoint/Services/RecherchePoint/RechercherPoint-v2.0.xsd` & `lowatt-enedis-2.2.1/lowatt_enedis/wsdl/RecherchePoint/Services/RecherchePoint/RechercherPoint-v2.0.xsd`

 * *Files identical despite different names*

### Comparing `lowatt-enedis-2.2.0/lowatt_enedis/wsdl/RechercheServicesSouscritsMesures/Dictionnaires/Metier/v5.0/ENEDIS.Dictionnaire.TypeComplexe.v5.0.xsd` & `lowatt-enedis-2.2.1/lowatt_enedis/wsdl/RechercheServicesSouscritsMesures/Dictionnaires/Metier/v5.0/ENEDIS.Dictionnaire.TypeComplexe.v5.0.xsd`

 * *Files identical despite different names*

### Comparing `lowatt-enedis-2.2.0/lowatt_enedis/wsdl/RechercheServicesSouscritsMesures/Dictionnaires/Metier/v5.0/ENEDIS.Dictionnaire.TypeSimple.v5.0.xsd` & `lowatt-enedis-2.2.1/lowatt_enedis/wsdl/RechercheServicesSouscritsMesures/Dictionnaires/Metier/v5.0/ENEDIS.Dictionnaire.TypeSimple.v5.0.xsd`

 * *Files identical despite different names*

### Comparing `lowatt-enedis-2.2.0/lowatt_enedis/wsdl/RechercheServicesSouscritsMesures/Dictionnaires/Technique/W3C.SoapEnv.xsd` & `lowatt-enedis-2.2.1/lowatt_enedis/wsdl/RechercheServicesSouscritsMesures/Dictionnaires/Technique/W3C.SoapEnv.xsd`

 * *Files identical despite different names*

### Comparing `lowatt-enedis-2.2.0/lowatt_enedis/wsdl/RechercheServicesSouscritsMesures/Dictionnaires/Technique/v1.0/ENEDIS.Dictionnaire.Technique.v1.0.xsd` & `lowatt-enedis-2.2.1/lowatt_enedis/wsdl/RechercheServicesSouscritsMesures/Dictionnaires/Technique/v1.0/ENEDIS.Dictionnaire.Technique.v1.0.xsd`

 * *Files identical despite different names*

### Comparing `lowatt-enedis-2.2.0/lowatt_enedis/wsdl/RechercheServicesSouscritsMesures/Services/RechercheServicesSouscritsMesures/RechercherServicesSouscritsMesures-v1.0.wsdl` & `lowatt-enedis-2.2.1/lowatt_enedis/wsdl/RechercheServicesSouscritsMesures/Services/RechercheServicesSouscritsMesures/RechercherServicesSouscritsMesures-v1.0.wsdl`

 * *Files identical despite different names*

### Comparing `lowatt-enedis-2.2.0/lowatt_enedis/wsdl/RechercheServicesSouscritsMesures/Services/RechercheServicesSouscritsMesures/RechercherServicesSouscritsMesures-v1.0.xsd` & `lowatt-enedis-2.2.1/lowatt_enedis/wsdl/RechercheServicesSouscritsMesures/Services/RechercheServicesSouscritsMesures/RechercherServicesSouscritsMesures-v1.0.xsd`

 * *Files identical despite different names*

### Comparing `lowatt-enedis-2.2.0/lowatt_enedis/wsdl/TransmissionHistoriqueMesures/Dictionnaires/v4.0/ERDF.Dictionnaire.TypeComplexe.v4.0.xsd` & `lowatt-enedis-2.2.1/lowatt_enedis/wsdl/TransmissionHistoriqueMesures/Dictionnaires/v4.0/ERDF.Dictionnaire.TypeComplexe.v4.0.xsd`

 * *Files identical despite different names*

### Comparing `lowatt-enedis-2.2.0/lowatt_enedis/wsdl/TransmissionHistoriqueMesures/Dictionnaires/v4.0/ERDF.Dictionnaire.TypeSimple.v4.0.xsd` & `lowatt-enedis-2.2.1/lowatt_enedis/wsdl/TransmissionHistoriqueMesures/Dictionnaires/v4.0/ERDF.Dictionnaire.TypeSimple.v4.0.xsd`

 * *Files identical despite different names*

### Comparing `lowatt-enedis-2.2.0/lowatt_enedis/wsdl/TransmissionHistoriqueMesures/Services/TransmissionHistoriqueMesures/CommandeTransmissionHistoriqueMesures-v1.0.wsdl` & `lowatt-enedis-2.2.1/lowatt_enedis/wsdl/TransmissionHistoriqueMesures/Services/TransmissionHistoriqueMesures/CommandeTransmissionHistoriqueMesures-v1.0.wsdl`

 * *Files identical despite different names*

### Comparing `lowatt-enedis-2.2.0/lowatt_enedis/wsdl/TransmissionHistoriqueMesures/Services/TransmissionHistoriqueMesures/CommanderTransmissionHistoriqueMesures-v1.0.xsd` & `lowatt-enedis-2.2.1/lowatt_enedis/wsdl/TransmissionHistoriqueMesures/Services/TransmissionHistoriqueMesures/CommanderTransmissionHistoriqueMesures-v1.0.xsd`

 * *Files identical despite different names*

### Comparing `lowatt-enedis-2.2.0/lowatt_enedis.egg-info/PKG-INFO` & `lowatt-enedis-2.2.1/lowatt_enedis.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lowatt-enedis
-Version: 2.2.0
+Version: 2.2.1
 Summary: Query Enedis SGE web-service
 Home-page: https://github.com/lowatt/lowatt-enedis
 Author: Lowatt
 Author-email: info@lowatt.fr
 License: GPL3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `lowatt-enedis-2.2.0/lowatt_enedis.egg-info/SOURCES.txt` & `lowatt-enedis-2.2.1/lowatt_enedis.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `lowatt-enedis-2.2.0/setup.cfg` & `lowatt-enedis-2.2.1/setup.cfg`

 * *Files 11% similar despite different names*

```diff
@@ -18,14 +18,15 @@
 [options]
 setup_requires = 
 	setuptools_scm
 python_requires = >=3.9
 packages = find:
 install_requires = 
 	python-dateutil
+	certifi
 	suds-py3
 include_package_data = True
 
 [options.extras_require]
 test = 
 	pytest
 	pytest-cov
```

### Comparing `lowatt-enedis-2.2.0/setup.py` & `lowatt-enedis-2.2.1/setup.py`

 * *Files identical despite different names*

### Comparing `lowatt-enedis-2.2.0/test/data/consulterMesuresDetailleesResponse.xml` & `lowatt-enedis-2.2.1/test/data/consulterMesuresDetailleesResponse.xml`

 * *Files identical despite different names*

### Comparing `lowatt-enedis-2.2.0/test/data/consulterMesuresResponse.xml` & `lowatt-enedis-2.2.1/test/data/consulterMesuresResponse.xml`

 * *Files identical despite different names*

### Comparing `lowatt-enedis-2.2.0/test/data/requests.yaml` & `lowatt-enedis-2.2.1/test/data/requests.yaml`

 * *Files identical despite different names*

### Comparing `lowatt-enedis-2.2.0/test/test_lowatt_enedis.py` & `lowatt-enedis-2.2.1/test/test_lowatt_enedis.py`

 * *Files identical despite different names*

### Comparing `lowatt-enedis-2.2.0/test/test_requests.py` & `lowatt-enedis-2.2.1/test/test_requests.py`

 * *Files identical despite different names*

### Comparing `lowatt-enedis-2.2.0/tox.ini` & `lowatt-enedis-2.2.1/tox.ini`

 * *Files identical despite different names*

