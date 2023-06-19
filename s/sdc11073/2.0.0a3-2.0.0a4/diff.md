# Comparing `tmp/sdc11073-2.0.0a3.tar.gz` & `tmp/sdc11073-2.0.0a4.tar.gz`

## Comparing `sdc11073-2.0.0a3.tar` & `sdc11073-2.0.0a4.tar`

### file list

```diff
@@ -1,134 +1,138 @@
--rw-r--r--   0        0        0     2146 2020-02-02 00:00:00.000000 sdc11073-2.0.0a3/CHANGELOG.md
--rw-r--r--   0        0        0   347063 2020-02-02 00:00:00.000000 sdc11073-2.0.0a3/docs/sdc_social_preview.jpg
--rw-r--r--   0        0        0      183 2020-02-02 00:00:00.000000 sdc11073-2.0.0a3/src/sdc11073/__init__.py
--rw-r--r--   0        0        0     3640 2020-02-02 00:00:00.000000 sdc11073-2.0.0a3/src/sdc11073/certloader.py
--rw-r--r--   0        0        0     3721 2020-02-02 00:00:00.000000 sdc11073-2.0.0a3/src/sdc11073/commlog.py
--rw-r--r--   0        0        0     3664 2020-02-02 00:00:00.000000 sdc11073-2.0.0a3/src/sdc11073/definitions_base.py
--rw-r--r--   0        0        0     1779 2020-02-02 00:00:00.000000 sdc11073-2.0.0a3/src/sdc11073/definitions_sdc.py
--rw-r--r--   0        0        0      633 2020-02-02 00:00:00.000000 sdc11073-2.0.0a3/src/sdc11073/etc.py
--rw-r--r--   0        0        0     1814 2020-02-02 00:00:00.000000 sdc11073-2.0.0a3/src/sdc11073/exceptions.py
--rw-r--r--   0        0        0     5148 2020-02-02 00:00:00.000000 sdc11073-2.0.0a3/src/sdc11073/location.py
--rw-r--r--   0        0        0     8723 2020-02-02 00:00:00.000000 sdc11073-2.0.0a3/src/sdc11073/loghelper.py
--rw-r--r--   0        0        0     9314 2020-02-02 00:00:00.000000 sdc11073-2.0.0a3/src/sdc11073/multikey.py
--rw-r--r--   0        0        0    10165 2020-02-02 00:00:00.000000 sdc11073-2.0.0a3/src/sdc11073/namespaces.py
--rw-r--r--   0        0        0     2911 2020-02-02 00:00:00.000000 sdc11073-2.0.0a3/src/sdc11073/schema_resolver.py
--rw-r--r--   0        0        0    51437 2020-02-02 00:00:00.000000 sdc11073-2.0.0a3/src/sdc11073/wsdiscovery.py
--rw-r--r--   0        0        0      200 2020-02-02 00:00:00.000000 sdc11073-2.0.0a3/src/sdc11073/dispatch/__init__.py
--rw-r--r--   0        0        0     3932 2020-02-02 00:00:00.000000 sdc11073-2.0.0a3/src/sdc11073/dispatch/dispatchkey.py
--rw-r--r--   0        0        0     4960 2020-02-02 00:00:00.000000 sdc11073-2.0.0a3/src/sdc11073/dispatch/messageconverter.py
--rw-r--r--   0        0        0      953 2020-02-02 00:00:00.000000 sdc11073-2.0.0a3/src/sdc11073/dispatch/pathelementregistry.py
--rw-r--r--   0        0        0     1282 2020-02-02 00:00:00.000000 sdc11073-2.0.0a3/src/sdc11073/dispatch/request.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sdc11073-2.0.0a3/src/sdc11073/httpserver/__init__.py
--rw-r--r--   0        0        0     4596 2020-02-02 00:00:00.000000 sdc11073-2.0.0a3/src/sdc11073/httpserver/compression.py
--rw-r--r--   0        0        0     6689 2020-02-02 00:00:00.000000 sdc11073-2.0.0a3/src/sdc11073/httpserver/httpreader.py
--rw-r--r--   0        0        0     5871 2020-02-02 00:00:00.000000 sdc11073-2.0.0a3/src/sdc11073/httpserver/httprequesthandler.py
--rw-r--r--   0        0        0     6312 2020-02-02 00:00:00.000000 sdc11073-2.0.0a3/src/sdc11073/httpserver/httpserverimpl.py
--rw-r--r--   0        0        0      153 2020-02-02 00:00:00.000000 sdc11073-2.0.0a3/src/sdc11073/mdib/__init__.py
--rw-r--r--   0        0        0    35169 2020-02-02 00:00:00.000000 sdc11073-2.0.0a3/src/sdc11073/mdib/clientmdib.py
--rw-r--r--   0        0        0    18950 2020-02-02 00:00:00.000000 sdc11073-2.0.0a3/src/sdc11073/mdib/clientmdibxtra.py
--rw-r--r--   0        0        0     6170 2020-02-02 00:00:00.000000 sdc11073-2.0.0a3/src/sdc11073/mdib/containerbase.py
--rw-r--r--   0        0        0    35160 2020-02-02 00:00:00.000000 sdc11073-2.0.0a3/src/sdc11073/mdib/descriptorcontainers.py
--rw-r--r--   0        0        0     8358 2020-02-02 00:00:00.000000 sdc11073-2.0.0a3/src/sdc11073/mdib/devicemdib.py
--rw-r--r--   0        0        0    14455 2020-02-02 00:00:00.000000 sdc11073-2.0.0a3/src/sdc11073/mdib/devicemdibxtra.py
--rw-r--r--   0        0        0    11662 2020-02-02 00:00:00.000000 sdc11073-2.0.0a3/src/sdc11073/mdib/devicewaveform.py
--rw-r--r--   0        0        0    25440 2020-02-02 00:00:00.000000 sdc11073-2.0.0a3/src/sdc11073/mdib/mdibbase.py
--rw-r--r--   0        0        0    24434 2020-02-02 00:00:00.000000 sdc11073-2.0.0a3/src/sdc11073/mdib/statecontainers.py
--rw-r--r--   0        0        0    36856 2020-02-02 00:00:00.000000 sdc11073-2.0.0a3/src/sdc11073/mdib/transactions.py
--rw-r--r--   0        0        0      822 2020-02-02 00:00:00.000000 sdc11073-2.0.0a3/src/sdc11073/netconn/__init__.py
--rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 sdc11073-2.0.0a3/src/sdc11073/observableproperties/__init__.py
--rw-r--r--   0        0        0     8027 2020-02-02 00:00:00.000000 sdc11073-2.0.0a3/src/sdc11073/observableproperties/observables.py
--rw-r--r--   0        0        0     3759 2020-02-02 00:00:00.000000 sdc11073-2.0.0a3/src/sdc11073/observableproperties/valuecollector.py
--rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 sdc11073-2.0.0a3/src/sdc11073/pysoap/__init__.py
--rw-r--r--   0        0        0     5687 2020-02-02 00:00:00.000000 sdc11073-2.0.0a3/src/sdc11073/pysoap/msgfactory.py
--rw-r--r--   0        0        0    10118 2020-02-02 00:00:00.000000 sdc11073-2.0.0a3/src/sdc11073/pysoap/msgreader.py
--rw-r--r--   0        0        0    15675 2020-02-02 00:00:00.000000 sdc11073-2.0.0a3/src/sdc11073/pysoap/soapclient.py
--rw-r--r--   0        0        0     7056 2020-02-02 00:00:00.000000 sdc11073-2.0.0a3/src/sdc11073/pysoap/soapclient_async.py
--rw-r--r--   0        0        0     3198 2020-02-02 00:00:00.000000 sdc11073-2.0.0a3/src/sdc11073/pysoap/soapclientpool.py
--rw-r--r--   0        0        0     5564 2020-02-02 00:00:00.000000 sdc11073-2.0.0a3/src/sdc11073/pysoap/soapenvelope.py
--rw-r--r--   0        0        0      271 2020-02-02 00:00:00.000000 sdc11073-2.0.0a3/src/sdc11073/roles/__init__.py
--rw-r--r--   0        0        0    21522 2020-02-02 00:00:00.000000 sdc11073-2.0.0a3/src/sdc11073/roles/alarmprovider.py
--rw-r--r--   0        0        0    13474 2020-02-02 00:00:00.000000 sdc11073-2.0.0a3/src/sdc11073/roles/audiopauseprovider.py
--rw-r--r--   0        0        0     9426 2020-02-02 00:00:00.000000 sdc11073-2.0.0a3/src/sdc11073/roles/clockprovider.py
--rw-r--r--   0        0        0     5377 2020-02-02 00:00:00.000000 sdc11073-2.0.0a3/src/sdc11073/roles/contextprovider.py
--rw-r--r--   0        0        0     6437 2020-02-02 00:00:00.000000 sdc11073-2.0.0a3/src/sdc11073/roles/metricprovider.py
--rw-r--r--   0        0        0      790 2020-02-02 00:00:00.000000 sdc11073-2.0.0a3/src/sdc11073/roles/nomenclature.py
--rw-r--r--   0        0        0      216 2020-02-02 00:00:00.000000 sdc11073-2.0.0a3/src/sdc11073/roles/operationprovider.py
--rw-r--r--   0        0        0     2511 2020-02-02 00:00:00.000000 sdc11073-2.0.0a3/src/sdc11073/roles/patientcontextprovider.py
--rw-r--r--   0        0        0    12539 2020-02-02 00:00:00.000000 sdc11073-2.0.0a3/src/sdc11073/roles/product.py
--rw-r--r--   0        0        0     7558 2020-02-02 00:00:00.000000 sdc11073-2.0.0a3/src/sdc11073/roles/providerbase.py
--rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 sdc11073-2.0.0a3/src/sdc11073/sdcclient/__init__.py
--rw-r--r--   0        0        0     2879 2020-02-02 00:00:00.000000 sdc11073-2.0.0a3/src/sdc11073/sdcclient/components.py
--rw-r--r--   0        0        0     1040 2020-02-02 00:00:00.000000 sdc11073-2.0.0a3/src/sdc11073/sdcclient/manipulator.py
--rw-r--r--   0        0        0     4373 2020-02-02 00:00:00.000000 sdc11073-2.0.0a3/src/sdc11073/sdcclient/operations.py
--rw-r--r--   0        0        0     1999 2020-02-02 00:00:00.000000 sdc11073-2.0.0a3/src/sdc11073/sdcclient/request_handler_deferred.py
--rw-r--r--   0        0        0    32203 2020-02-02 00:00:00.000000 sdc11073-2.0.0a3/src/sdc11073/sdcclient/sdcclientimpl.py
--rw-r--r--   0        0        0    22009 2020-02-02 00:00:00.000000 sdc11073-2.0.0a3/src/sdc11073/sdcclient/subscription.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sdc11073-2.0.0a3/src/sdc11073/sdcclient/serviceclients/__init__.py
--rw-r--r--   0        0        0     2378 2020-02-02 00:00:00.000000 sdc11073-2.0.0a3/src/sdc11073/sdcclient/serviceclients/containmenttreeservice.py
--rw-r--r--   0        0        0     6757 2020-02-02 00:00:00.000000 sdc11073-2.0.0a3/src/sdc11073/sdcclient/serviceclients/contextservice.py
--rw-r--r--   0        0        0      441 2020-02-02 00:00:00.000000 sdc11073-2.0.0a3/src/sdc11073/sdcclient/serviceclients/descriptioneventservice.py
--rw-r--r--   0        0        0     3234 2020-02-02 00:00:00.000000 sdc11073-2.0.0a3/src/sdc11073/sdcclient/serviceclients/getservice.py
--rw-r--r--   0        0        0     2393 2020-02-02 00:00:00.000000 sdc11073-2.0.0a3/src/sdc11073/sdcclient/serviceclients/localizationservice.py
--rw-r--r--   0        0        0     4378 2020-02-02 00:00:00.000000 sdc11073-2.0.0a3/src/sdc11073/sdcclient/serviceclients/serviceclientbase.py
--rw-r--r--   0        0        0     8291 2020-02-02 00:00:00.000000 sdc11073-2.0.0a3/src/sdc11073/sdcclient/serviceclients/setservice.py
--rw-r--r--   0        0        0     1160 2020-02-02 00:00:00.000000 sdc11073-2.0.0a3/src/sdc11073/sdcclient/serviceclients/stateeventservice.py
--rw-r--r--   0        0        0      389 2020-02-02 00:00:00.000000 sdc11073-2.0.0a3/src/sdc11073/sdcclient/serviceclients/waveformservice.py
--rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 sdc11073-2.0.0a3/src/sdc11073/sdcdevice/__init__.py
--rw-r--r--   0        0        0     4986 2020-02-02 00:00:00.000000 sdc11073-2.0.0a3/src/sdc11073/sdcdevice/components.py
--rw-r--r--   0        0        0     9360 2020-02-02 00:00:00.000000 sdc11073-2.0.0a3/src/sdc11073/sdcdevice/dpwshostedservice.py
--rw-r--r--   0        0        0     1260 2020-02-02 00:00:00.000000 sdc11073-2.0.0a3/src/sdc11073/sdcdevice/intervaltimer.py
--rw-r--r--   0        0        0     5282 2020-02-02 00:00:00.000000 sdc11073-2.0.0a3/src/sdc11073/sdcdevice/operations.py
--rw-r--r--   0        0        0    10632 2020-02-02 00:00:00.000000 sdc11073-2.0.0a3/src/sdc11073/sdcdevice/periodicreports.py
--rw-r--r--   0        0        0    16697 2020-02-02 00:00:00.000000 sdc11073-2.0.0a3/src/sdc11073/sdcdevice/sco.py
--rw-r--r--   0        0        0     3068 2020-02-02 00:00:00.000000 sdc11073-2.0.0a3/src/sdc11073/sdcdevice/scopesfactory.py
--rw-r--r--   0        0        0    24480 2020-02-02 00:00:00.000000 sdc11073-2.0.0a3/src/sdc11073/sdcdevice/sdcdeviceimpl.py
--rw-r--r--   0        0        0     2753 2020-02-02 00:00:00.000000 sdc11073-2.0.0a3/src/sdc11073/sdcdevice/servicesfactory.py
--rw-r--r--   0        0        0     4284 2020-02-02 00:00:00.000000 sdc11073-2.0.0a3/src/sdc11073/sdcdevice/subscriptionmgr.py
--rw-r--r--   0        0        0    14883 2020-02-02 00:00:00.000000 sdc11073-2.0.0a3/src/sdc11073/sdcdevice/subscriptionmgr_async.py
--rw-r--r--   0        0        0    24606 2020-02-02 00:00:00.000000 sdc11073-2.0.0a3/src/sdc11073/sdcdevice/subscriptionmgr_base.py
--rw-r--r--   0        0        0     5557 2020-02-02 00:00:00.000000 sdc11073-2.0.0a3/src/sdc11073/sdcdevice/waveforms.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sdc11073-2.0.0a3/src/sdc11073/sdcdevice/porttypes/__init__.py
--rw-r--r--   0        0        0     2896 2020-02-02 00:00:00.000000 sdc11073-2.0.0a3/src/sdc11073/sdcdevice/porttypes/containmenttreeserviceimpl.py
--rw-r--r--   0        0        0     8163 2020-02-02 00:00:00.000000 sdc11073-2.0.0a3/src/sdc11073/sdcdevice/porttypes/contextserviceimpl.py
--rw-r--r--   0        0        0     3861 2020-02-02 00:00:00.000000 sdc11073-2.0.0a3/src/sdc11073/sdcdevice/porttypes/descriptioneventserviceimpl.py
--rw-r--r--   0        0        0     9304 2020-02-02 00:00:00.000000 sdc11073-2.0.0a3/src/sdc11073/sdcdevice/porttypes/getserviceimpl.py
--rw-r--r--   0        0        0    12617 2020-02-02 00:00:00.000000 sdc11073-2.0.0a3/src/sdc11073/sdcdevice/porttypes/localizationservice.py
--rw-r--r--   0        0        0    12227 2020-02-02 00:00:00.000000 sdc11073-2.0.0a3/src/sdc11073/sdcdevice/porttypes/porttypebase.py
--rw-r--r--   0        0        0    11710 2020-02-02 00:00:00.000000 sdc11073-2.0.0a3/src/sdc11073/sdcdevice/porttypes/setserviceimpl.py
--rw-r--r--   0        0        0    10505 2020-02-02 00:00:00.000000 sdc11073-2.0.0a3/src/sdc11073/sdcdevice/porttypes/stateeventserviceimpl.py
--rw-r--r--   0        0        0     1722 2020-02-02 00:00:00.000000 sdc11073-2.0.0a3/src/sdc11073/sdcdevice/porttypes/waveformserviceimpl.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sdc11073-2.0.0a3/src/sdc11073/xml_types/__init__.py
--rw-r--r--   0        0        0     4497 2020-02-02 00:00:00.000000 sdc11073-2.0.0a3/src/sdc11073/xml_types/actions.py
--rw-r--r--   0        0        0     4635 2020-02-02 00:00:00.000000 sdc11073-2.0.0a3/src/sdc11073/xml_types/addressing_types.py
--rw-r--r--   0        0        0     4705 2020-02-02 00:00:00.000000 sdc11073-2.0.0a3/src/sdc11073/xml_types/basetypes.py
--rw-r--r--   0        0        0     7907 2020-02-02 00:00:00.000000 sdc11073-2.0.0a3/src/sdc11073/xml_types/dataconverters.py
--rw-r--r--   0        0        0     6365 2020-02-02 00:00:00.000000 sdc11073-2.0.0a3/src/sdc11073/xml_types/dpws_types.py
--rw-r--r--   0        0        0     5230 2020-02-02 00:00:00.000000 sdc11073-2.0.0a3/src/sdc11073/xml_types/eventing_types.py
--rw-r--r--   0        0        0      192 2020-02-02 00:00:00.000000 sdc11073-2.0.0a3/src/sdc11073/xml_types/ext_qnames.py
--rw-r--r--   0        0        0     7719 2020-02-02 00:00:00.000000 sdc11073-2.0.0a3/src/sdc11073/xml_types/isoduration.py
--rw-r--r--   0        0        0     5723 2020-02-02 00:00:00.000000 sdc11073-2.0.0a3/src/sdc11073/xml_types/mex_types.py
--rw-r--r--   0        0        0     7602 2020-02-02 00:00:00.000000 sdc11073-2.0.0a3/src/sdc11073/xml_types/msg_qnames.py
--rw-r--r--   0        0        0    27781 2020-02-02 00:00:00.000000 sdc11073-2.0.0a3/src/sdc11073/xml_types/msg_types.py
--rw-r--r--   0        0        0    15580 2020-02-02 00:00:00.000000 sdc11073-2.0.0a3/src/sdc11073/xml_types/pm_qnames.py
--rw-r--r--   0        0        0    58377 2020-02-02 00:00:00.000000 sdc11073-2.0.0a3/src/sdc11073/xml_types/pm_types.py
--rw-r--r--   0        0        0     6509 2020-02-02 00:00:00.000000 sdc11073-2.0.0a3/src/sdc11073/xml_types/wsd_types.py
--rw-r--r--   0        0        0    53115 2020-02-02 00:00:00.000000 sdc11073-2.0.0a3/src/sdc11073/xml_types/xml_structure.py
--rw-r--r--   0        0        0    75099 2020-02-02 00:00:00.000000 sdc11073-2.0.0a3/src/sdc11073/xsd/BICEPS_MessageModel.xsd
--rw-r--r--   0        0        0   205547 2020-02-02 00:00:00.000000 sdc11073-2.0.0a3/src/sdc11073/xsd/BICEPS_ParticipantModel.xsd
--rw-r--r--   0        0        0     1499 2020-02-02 00:00:00.000000 sdc11073-2.0.0a3/src/sdc11073/xsd/ExtensionPoint.xsd
--rw-r--r--   0        0        0     4361 2020-02-02 00:00:00.000000 sdc11073-2.0.0a3/src/sdc11073/xsd/MetadataExchange.xsd
--rw-r--r--   0        0        0     9037 2020-02-02 00:00:00.000000 sdc11073-2.0.0a3/src/sdc11073/xsd/SafetyInformation.xsd
--rw-r--r--   0        0        0     7127 2020-02-02 00:00:00.000000 sdc11073-2.0.0a3/src/sdc11073/xsd/addressing.xsd
--rw-r--r--   0        0        0     9275 2020-02-02 00:00:00.000000 sdc11073-2.0.0a3/src/sdc11073/xsd/eventing.xsd
--rw-r--r--   0        0        0     5618 2020-02-02 00:00:00.000000 sdc11073-2.0.0a3/src/sdc11073/xsd/soap-envelope.xsd
--rw-r--r--   0        0        0     5573 2020-02-02 00:00:00.000000 sdc11073-2.0.0a3/src/sdc11073/xsd/ws-addr.xsd
--rw-r--r--   0        0        0    11535 2020-02-02 00:00:00.000000 sdc11073-2.0.0a3/src/sdc11073/xsd/wsdd-discovery-1.1-schema-os.xsd
--rw-r--r--   0        0        0     9881 2020-02-02 00:00:00.000000 sdc11073-2.0.0a3/src/sdc11073/xsd/wsdd-dpws-1.1-schema-os.xsd
--rw-r--r--   0        0        0    11591 2020-02-02 00:00:00.000000 sdc11073-2.0.0a3/src/sdc11073/xsd/wsdl.xsd
--rw-r--r--   0        0        0     1684 2020-02-02 00:00:00.000000 sdc11073-2.0.0a3/src/sdc11073/xsd/xml.xsd
--rw-r--r--   0        0        0      549 2020-02-02 00:00:00.000000 sdc11073-2.0.0a3/tutorial/README.rst
--rw-r--r--   0        0        0     1805 2020-02-02 00:00:00.000000 sdc11073-2.0.0a3/.gitignore
--rw-r--r--   0        0        0     1064 2020-02-02 00:00:00.000000 sdc11073-2.0.0a3/LICENSE
--rw-r--r--   0        0        0     2344 2020-02-02 00:00:00.000000 sdc11073-2.0.0a3/README.rst
--rw-r--r--   0        0        0     5652 2020-02-02 00:00:00.000000 sdc11073-2.0.0a3/pyproject.toml
--rw-r--r--   0        0        0     3573 2020-02-02 00:00:00.000000 sdc11073-2.0.0a3/PKG-INFO
+-rw-r--r--   0        0        0     2582 2020-02-02 00:00:00.000000 sdc11073-2.0.0a4/CHANGELOG.md
+-rw-r--r--   0        0        0   347063 2020-02-02 00:00:00.000000 sdc11073-2.0.0a4/docs/sdc_social_preview.jpg
+-rw-r--r--   0        0        0      183 2020-02-02 00:00:00.000000 sdc11073-2.0.0a4/src/sdc11073/__init__.py
+-rw-r--r--   0        0        0     3640 2020-02-02 00:00:00.000000 sdc11073-2.0.0a4/src/sdc11073/certloader.py
+-rw-r--r--   0        0        0     3721 2020-02-02 00:00:00.000000 sdc11073-2.0.0a4/src/sdc11073/commlog.py
+-rw-r--r--   0        0        0     3664 2020-02-02 00:00:00.000000 sdc11073-2.0.0a4/src/sdc11073/definitions_base.py
+-rw-r--r--   0        0        0     1779 2020-02-02 00:00:00.000000 sdc11073-2.0.0a4/src/sdc11073/definitions_sdc.py
+-rw-r--r--   0        0        0      633 2020-02-02 00:00:00.000000 sdc11073-2.0.0a4/src/sdc11073/etc.py
+-rw-r--r--   0        0        0     1814 2020-02-02 00:00:00.000000 sdc11073-2.0.0a4/src/sdc11073/exceptions.py
+-rw-r--r--   0        0        0     5148 2020-02-02 00:00:00.000000 sdc11073-2.0.0a4/src/sdc11073/location.py
+-rw-r--r--   0        0        0     8772 2020-02-02 00:00:00.000000 sdc11073-2.0.0a4/src/sdc11073/loghelper.py
+-rw-r--r--   0        0        0     9314 2020-02-02 00:00:00.000000 sdc11073-2.0.0a4/src/sdc11073/multikey.py
+-rw-r--r--   0        0        0    10165 2020-02-02 00:00:00.000000 sdc11073-2.0.0a4/src/sdc11073/namespaces.py
+-rw-r--r--   0        0        0     2911 2020-02-02 00:00:00.000000 sdc11073-2.0.0a4/src/sdc11073/schema_resolver.py
+-rw-r--r--   0        0        0      200 2020-02-02 00:00:00.000000 sdc11073-2.0.0a4/src/sdc11073/dispatch/__init__.py
+-rw-r--r--   0        0        0     3932 2020-02-02 00:00:00.000000 sdc11073-2.0.0a4/src/sdc11073/dispatch/dispatchkey.py
+-rw-r--r--   0        0        0     4960 2020-02-02 00:00:00.000000 sdc11073-2.0.0a4/src/sdc11073/dispatch/messageconverter.py
+-rw-r--r--   0        0        0      953 2020-02-02 00:00:00.000000 sdc11073-2.0.0a4/src/sdc11073/dispatch/pathelementregistry.py
+-rw-r--r--   0        0        0     1282 2020-02-02 00:00:00.000000 sdc11073-2.0.0a4/src/sdc11073/dispatch/request.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sdc11073-2.0.0a4/src/sdc11073/httpserver/__init__.py
+-rw-r--r--   0        0        0     4596 2020-02-02 00:00:00.000000 sdc11073-2.0.0a4/src/sdc11073/httpserver/compression.py
+-rw-r--r--   0        0        0     6689 2020-02-02 00:00:00.000000 sdc11073-2.0.0a4/src/sdc11073/httpserver/httpreader.py
+-rw-r--r--   0        0        0     5871 2020-02-02 00:00:00.000000 sdc11073-2.0.0a4/src/sdc11073/httpserver/httprequesthandler.py
+-rw-r--r--   0        0        0     6312 2020-02-02 00:00:00.000000 sdc11073-2.0.0a4/src/sdc11073/httpserver/httpserverimpl.py
+-rw-r--r--   0        0        0      153 2020-02-02 00:00:00.000000 sdc11073-2.0.0a4/src/sdc11073/mdib/__init__.py
+-rw-r--r--   0        0        0    35169 2020-02-02 00:00:00.000000 sdc11073-2.0.0a4/src/sdc11073/mdib/clientmdib.py
+-rw-r--r--   0        0        0    19227 2020-02-02 00:00:00.000000 sdc11073-2.0.0a4/src/sdc11073/mdib/clientmdibxtra.py
+-rw-r--r--   0        0        0     6170 2020-02-02 00:00:00.000000 sdc11073-2.0.0a4/src/sdc11073/mdib/containerbase.py
+-rw-r--r--   0        0        0    35160 2020-02-02 00:00:00.000000 sdc11073-2.0.0a4/src/sdc11073/mdib/descriptorcontainers.py
+-rw-r--r--   0        0        0     8358 2020-02-02 00:00:00.000000 sdc11073-2.0.0a4/src/sdc11073/mdib/devicemdib.py
+-rw-r--r--   0        0        0    14455 2020-02-02 00:00:00.000000 sdc11073-2.0.0a4/src/sdc11073/mdib/devicemdibxtra.py
+-rw-r--r--   0        0        0    11662 2020-02-02 00:00:00.000000 sdc11073-2.0.0a4/src/sdc11073/mdib/devicewaveform.py
+-rw-r--r--   0        0        0    25440 2020-02-02 00:00:00.000000 sdc11073-2.0.0a4/src/sdc11073/mdib/mdibbase.py
+-rw-r--r--   0        0        0    24434 2020-02-02 00:00:00.000000 sdc11073-2.0.0a4/src/sdc11073/mdib/statecontainers.py
+-rw-r--r--   0        0        0    36856 2020-02-02 00:00:00.000000 sdc11073-2.0.0a4/src/sdc11073/mdib/transactions.py
+-rw-r--r--   0        0        0      822 2020-02-02 00:00:00.000000 sdc11073-2.0.0a4/src/sdc11073/netconn/__init__.py
+-rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 sdc11073-2.0.0a4/src/sdc11073/observableproperties/__init__.py
+-rw-r--r--   0        0        0     8027 2020-02-02 00:00:00.000000 sdc11073-2.0.0a4/src/sdc11073/observableproperties/observables.py
+-rw-r--r--   0        0        0     3759 2020-02-02 00:00:00.000000 sdc11073-2.0.0a4/src/sdc11073/observableproperties/valuecollector.py
+-rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 sdc11073-2.0.0a4/src/sdc11073/pysoap/__init__.py
+-rw-r--r--   0        0        0     5687 2020-02-02 00:00:00.000000 sdc11073-2.0.0a4/src/sdc11073/pysoap/msgfactory.py
+-rw-r--r--   0        0        0    10118 2020-02-02 00:00:00.000000 sdc11073-2.0.0a4/src/sdc11073/pysoap/msgreader.py
+-rw-r--r--   0        0        0    15907 2020-02-02 00:00:00.000000 sdc11073-2.0.0a4/src/sdc11073/pysoap/soapclient.py
+-rw-r--r--   0        0        0     7056 2020-02-02 00:00:00.000000 sdc11073-2.0.0a4/src/sdc11073/pysoap/soapclient_async.py
+-rw-r--r--   0        0        0     3198 2020-02-02 00:00:00.000000 sdc11073-2.0.0a4/src/sdc11073/pysoap/soapclientpool.py
+-rw-r--r--   0        0        0     5564 2020-02-02 00:00:00.000000 sdc11073-2.0.0a4/src/sdc11073/pysoap/soapenvelope.py
+-rw-r--r--   0        0        0      271 2020-02-02 00:00:00.000000 sdc11073-2.0.0a4/src/sdc11073/roles/__init__.py
+-rw-r--r--   0        0        0    21440 2020-02-02 00:00:00.000000 sdc11073-2.0.0a4/src/sdc11073/roles/alarmprovider.py
+-rw-r--r--   0        0        0    13474 2020-02-02 00:00:00.000000 sdc11073-2.0.0a4/src/sdc11073/roles/audiopauseprovider.py
+-rw-r--r--   0        0        0     9426 2020-02-02 00:00:00.000000 sdc11073-2.0.0a4/src/sdc11073/roles/clockprovider.py
+-rw-r--r--   0        0        0     5377 2020-02-02 00:00:00.000000 sdc11073-2.0.0a4/src/sdc11073/roles/contextprovider.py
+-rw-r--r--   0        0        0     6437 2020-02-02 00:00:00.000000 sdc11073-2.0.0a4/src/sdc11073/roles/metricprovider.py
+-rw-r--r--   0        0        0      790 2020-02-02 00:00:00.000000 sdc11073-2.0.0a4/src/sdc11073/roles/nomenclature.py
+-rw-r--r--   0        0        0      216 2020-02-02 00:00:00.000000 sdc11073-2.0.0a4/src/sdc11073/roles/operationprovider.py
+-rw-r--r--   0        0        0     2511 2020-02-02 00:00:00.000000 sdc11073-2.0.0a4/src/sdc11073/roles/patientcontextprovider.py
+-rw-r--r--   0        0        0    12539 2020-02-02 00:00:00.000000 sdc11073-2.0.0a4/src/sdc11073/roles/product.py
+-rw-r--r--   0        0        0     7558 2020-02-02 00:00:00.000000 sdc11073-2.0.0a4/src/sdc11073/roles/providerbase.py
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 sdc11073-2.0.0a4/src/sdc11073/sdcclient/__init__.py
+-rw-r--r--   0        0        0     2879 2020-02-02 00:00:00.000000 sdc11073-2.0.0a4/src/sdc11073/sdcclient/components.py
+-rw-r--r--   0        0        0     1040 2020-02-02 00:00:00.000000 sdc11073-2.0.0a4/src/sdc11073/sdcclient/manipulator.py
+-rw-r--r--   0        0        0     4373 2020-02-02 00:00:00.000000 sdc11073-2.0.0a4/src/sdc11073/sdcclient/operations.py
+-rw-r--r--   0        0        0     1999 2020-02-02 00:00:00.000000 sdc11073-2.0.0a4/src/sdc11073/sdcclient/request_handler_deferred.py
+-rw-r--r--   0        0        0    32197 2020-02-02 00:00:00.000000 sdc11073-2.0.0a4/src/sdc11073/sdcclient/sdcclientimpl.py
+-rw-r--r--   0        0        0    22009 2020-02-02 00:00:00.000000 sdc11073-2.0.0a4/src/sdc11073/sdcclient/subscription.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sdc11073-2.0.0a4/src/sdc11073/sdcclient/serviceclients/__init__.py
+-rw-r--r--   0        0        0     2378 2020-02-02 00:00:00.000000 sdc11073-2.0.0a4/src/sdc11073/sdcclient/serviceclients/containmenttreeservice.py
+-rw-r--r--   0        0        0     6757 2020-02-02 00:00:00.000000 sdc11073-2.0.0a4/src/sdc11073/sdcclient/serviceclients/contextservice.py
+-rw-r--r--   0        0        0      441 2020-02-02 00:00:00.000000 sdc11073-2.0.0a4/src/sdc11073/sdcclient/serviceclients/descriptioneventservice.py
+-rw-r--r--   0        0        0     3234 2020-02-02 00:00:00.000000 sdc11073-2.0.0a4/src/sdc11073/sdcclient/serviceclients/getservice.py
+-rw-r--r--   0        0        0     2393 2020-02-02 00:00:00.000000 sdc11073-2.0.0a4/src/sdc11073/sdcclient/serviceclients/localizationservice.py
+-rw-r--r--   0        0        0     4378 2020-02-02 00:00:00.000000 sdc11073-2.0.0a4/src/sdc11073/sdcclient/serviceclients/serviceclientbase.py
+-rw-r--r--   0        0        0     8291 2020-02-02 00:00:00.000000 sdc11073-2.0.0a4/src/sdc11073/sdcclient/serviceclients/setservice.py
+-rw-r--r--   0        0        0     1160 2020-02-02 00:00:00.000000 sdc11073-2.0.0a4/src/sdc11073/sdcclient/serviceclients/stateeventservice.py
+-rw-r--r--   0        0        0      389 2020-02-02 00:00:00.000000 sdc11073-2.0.0a4/src/sdc11073/sdcclient/serviceclients/waveformservice.py
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 sdc11073-2.0.0a4/src/sdc11073/sdcdevice/__init__.py
+-rw-r--r--   0        0        0     4938 2020-02-02 00:00:00.000000 sdc11073-2.0.0a4/src/sdc11073/sdcdevice/components.py
+-rw-r--r--   0        0        0     9360 2020-02-02 00:00:00.000000 sdc11073-2.0.0a4/src/sdc11073/sdcdevice/dpwshostedservice.py
+-rw-r--r--   0        0        0     1260 2020-02-02 00:00:00.000000 sdc11073-2.0.0a4/src/sdc11073/sdcdevice/intervaltimer.py
+-rw-r--r--   0        0        0     5282 2020-02-02 00:00:00.000000 sdc11073-2.0.0a4/src/sdc11073/sdcdevice/operations.py
+-rw-r--r--   0        0        0    10632 2020-02-02 00:00:00.000000 sdc11073-2.0.0a4/src/sdc11073/sdcdevice/periodicreports.py
+-rw-r--r--   0        0        0    16697 2020-02-02 00:00:00.000000 sdc11073-2.0.0a4/src/sdc11073/sdcdevice/sco.py
+-rw-r--r--   0        0        0     3068 2020-02-02 00:00:00.000000 sdc11073-2.0.0a4/src/sdc11073/sdcdevice/scopesfactory.py
+-rw-r--r--   0        0        0    24480 2020-02-02 00:00:00.000000 sdc11073-2.0.0a4/src/sdc11073/sdcdevice/sdcdeviceimpl.py
+-rw-r--r--   0        0        0     2753 2020-02-02 00:00:00.000000 sdc11073-2.0.0a4/src/sdc11073/sdcdevice/servicesfactory.py
+-rw-r--r--   0        0        0     4284 2020-02-02 00:00:00.000000 sdc11073-2.0.0a4/src/sdc11073/sdcdevice/subscriptionmgr.py
+-rw-r--r--   0        0        0    14883 2020-02-02 00:00:00.000000 sdc11073-2.0.0a4/src/sdc11073/sdcdevice/subscriptionmgr_async.py
+-rw-r--r--   0        0        0    24606 2020-02-02 00:00:00.000000 sdc11073-2.0.0a4/src/sdc11073/sdcdevice/subscriptionmgr_base.py
+-rw-r--r--   0        0        0     5557 2020-02-02 00:00:00.000000 sdc11073-2.0.0a4/src/sdc11073/sdcdevice/waveforms.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sdc11073-2.0.0a4/src/sdc11073/sdcdevice/porttypes/__init__.py
+-rw-r--r--   0        0        0     2896 2020-02-02 00:00:00.000000 sdc11073-2.0.0a4/src/sdc11073/sdcdevice/porttypes/containmenttreeserviceimpl.py
+-rw-r--r--   0        0        0     8163 2020-02-02 00:00:00.000000 sdc11073-2.0.0a4/src/sdc11073/sdcdevice/porttypes/contextserviceimpl.py
+-rw-r--r--   0        0        0     3861 2020-02-02 00:00:00.000000 sdc11073-2.0.0a4/src/sdc11073/sdcdevice/porttypes/descriptioneventserviceimpl.py
+-rw-r--r--   0        0        0     9304 2020-02-02 00:00:00.000000 sdc11073-2.0.0a4/src/sdc11073/sdcdevice/porttypes/getserviceimpl.py
+-rw-r--r--   0        0        0    12617 2020-02-02 00:00:00.000000 sdc11073-2.0.0a4/src/sdc11073/sdcdevice/porttypes/localizationservice.py
+-rw-r--r--   0        0        0    12227 2020-02-02 00:00:00.000000 sdc11073-2.0.0a4/src/sdc11073/sdcdevice/porttypes/porttypebase.py
+-rw-r--r--   0        0        0    11710 2020-02-02 00:00:00.000000 sdc11073-2.0.0a4/src/sdc11073/sdcdevice/porttypes/setserviceimpl.py
+-rw-r--r--   0        0        0    10505 2020-02-02 00:00:00.000000 sdc11073-2.0.0a4/src/sdc11073/sdcdevice/porttypes/stateeventserviceimpl.py
+-rw-r--r--   0        0        0     1722 2020-02-02 00:00:00.000000 sdc11073-2.0.0a4/src/sdc11073/sdcdevice/porttypes/waveformserviceimpl.py
+-rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 sdc11073-2.0.0a4/src/sdc11073/wsdiscovery/__init__.py
+-rw-r--r--   0        0        0      522 2020-02-02 00:00:00.000000 sdc11073-2.0.0a4/src/sdc11073/wsdiscovery/common.py
+-rw-r--r--   0        0        0    15476 2020-02-02 00:00:00.000000 sdc11073-2.0.0a4/src/sdc11073/wsdiscovery/networkingthread.py
+-rw-r--r--   0        0        0     2129 2020-02-02 00:00:00.000000 sdc11073-2.0.0a4/src/sdc11073/wsdiscovery/service.py
+-rw-r--r--   0        0        0    30230 2020-02-02 00:00:00.000000 sdc11073-2.0.0a4/src/sdc11073/wsdiscovery/wsdimpl.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sdc11073-2.0.0a4/src/sdc11073/xml_types/__init__.py
+-rw-r--r--   0        0        0     4497 2020-02-02 00:00:00.000000 sdc11073-2.0.0a4/src/sdc11073/xml_types/actions.py
+-rw-r--r--   0        0        0     4698 2020-02-02 00:00:00.000000 sdc11073-2.0.0a4/src/sdc11073/xml_types/addressing_types.py
+-rw-r--r--   0        0        0     4705 2020-02-02 00:00:00.000000 sdc11073-2.0.0a4/src/sdc11073/xml_types/basetypes.py
+-rw-r--r--   0        0        0     7907 2020-02-02 00:00:00.000000 sdc11073-2.0.0a4/src/sdc11073/xml_types/dataconverters.py
+-rw-r--r--   0        0        0     6365 2020-02-02 00:00:00.000000 sdc11073-2.0.0a4/src/sdc11073/xml_types/dpws_types.py
+-rw-r--r--   0        0        0     5230 2020-02-02 00:00:00.000000 sdc11073-2.0.0a4/src/sdc11073/xml_types/eventing_types.py
+-rw-r--r--   0        0        0      192 2020-02-02 00:00:00.000000 sdc11073-2.0.0a4/src/sdc11073/xml_types/ext_qnames.py
+-rw-r--r--   0        0        0     7719 2020-02-02 00:00:00.000000 sdc11073-2.0.0a4/src/sdc11073/xml_types/isoduration.py
+-rw-r--r--   0        0        0     5723 2020-02-02 00:00:00.000000 sdc11073-2.0.0a4/src/sdc11073/xml_types/mex_types.py
+-rw-r--r--   0        0        0     7602 2020-02-02 00:00:00.000000 sdc11073-2.0.0a4/src/sdc11073/xml_types/msg_qnames.py
+-rw-r--r--   0        0        0    27781 2020-02-02 00:00:00.000000 sdc11073-2.0.0a4/src/sdc11073/xml_types/msg_types.py
+-rw-r--r--   0        0        0    15580 2020-02-02 00:00:00.000000 sdc11073-2.0.0a4/src/sdc11073/xml_types/pm_qnames.py
+-rw-r--r--   0        0        0    58377 2020-02-02 00:00:00.000000 sdc11073-2.0.0a4/src/sdc11073/xml_types/pm_types.py
+-rw-r--r--   0        0        0     6509 2020-02-02 00:00:00.000000 sdc11073-2.0.0a4/src/sdc11073/xml_types/wsd_types.py
+-rw-r--r--   0        0        0    53115 2020-02-02 00:00:00.000000 sdc11073-2.0.0a4/src/sdc11073/xml_types/xml_structure.py
+-rw-r--r--   0        0        0    75099 2020-02-02 00:00:00.000000 sdc11073-2.0.0a4/src/sdc11073/xsd/BICEPS_MessageModel.xsd
+-rw-r--r--   0        0        0   205547 2020-02-02 00:00:00.000000 sdc11073-2.0.0a4/src/sdc11073/xsd/BICEPS_ParticipantModel.xsd
+-rw-r--r--   0        0        0     1499 2020-02-02 00:00:00.000000 sdc11073-2.0.0a4/src/sdc11073/xsd/ExtensionPoint.xsd
+-rw-r--r--   0        0        0     4361 2020-02-02 00:00:00.000000 sdc11073-2.0.0a4/src/sdc11073/xsd/MetadataExchange.xsd
+-rw-r--r--   0        0        0     9037 2020-02-02 00:00:00.000000 sdc11073-2.0.0a4/src/sdc11073/xsd/SafetyInformation.xsd
+-rw-r--r--   0        0        0     7127 2020-02-02 00:00:00.000000 sdc11073-2.0.0a4/src/sdc11073/xsd/addressing.xsd
+-rw-r--r--   0        0        0     9275 2020-02-02 00:00:00.000000 sdc11073-2.0.0a4/src/sdc11073/xsd/eventing.xsd
+-rw-r--r--   0        0        0     5618 2020-02-02 00:00:00.000000 sdc11073-2.0.0a4/src/sdc11073/xsd/soap-envelope.xsd
+-rw-r--r--   0        0        0     5573 2020-02-02 00:00:00.000000 sdc11073-2.0.0a4/src/sdc11073/xsd/ws-addr.xsd
+-rw-r--r--   0        0        0    11535 2020-02-02 00:00:00.000000 sdc11073-2.0.0a4/src/sdc11073/xsd/wsdd-discovery-1.1-schema-os.xsd
+-rw-r--r--   0        0        0     9881 2020-02-02 00:00:00.000000 sdc11073-2.0.0a4/src/sdc11073/xsd/wsdd-dpws-1.1-schema-os.xsd
+-rw-r--r--   0        0        0    11591 2020-02-02 00:00:00.000000 sdc11073-2.0.0a4/src/sdc11073/xsd/wsdl.xsd
+-rw-r--r--   0        0        0     1684 2020-02-02 00:00:00.000000 sdc11073-2.0.0a4/src/sdc11073/xsd/xml.xsd
+-rw-r--r--   0        0        0      549 2020-02-02 00:00:00.000000 sdc11073-2.0.0a4/tutorial/README.rst
+-rw-r--r--   0        0        0     1805 2020-02-02 00:00:00.000000 sdc11073-2.0.0a4/.gitignore
+-rw-r--r--   0        0        0     1064 2020-02-02 00:00:00.000000 sdc11073-2.0.0a4/LICENSE
+-rw-r--r--   0        0        0     2522 2020-02-02 00:00:00.000000 sdc11073-2.0.0a4/README.rst
+-rw-r--r--   0        0        0     5652 2020-02-02 00:00:00.000000 sdc11073-2.0.0a4/pyproject.toml
+-rw-r--r--   0        0        0     3751 2020-02-02 00:00:00.000000 sdc11073-2.0.0a4/PKG-INFO
```

### Comparing `sdc11073-2.0.0a3/CHANGELOG.md` & `sdc11073-2.0.0a4/CHANGELOG.md`

 * *Files 10% similar despite different names*

```diff
@@ -3,14 +3,25 @@
 All notable changes to the sdc11073 module will be documented in this file.
 
 The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
 and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).
 
 ## [master]
 
+## [2.0.0a4] - 2023-06-16
+
+### Changed
+- reworked wsdiscovery. Wsdiscovery can now only bind to a single ip address. 
+  The only available classes are "WsDiscovery" and "WsDiscoverySingleAdapter".
+
+### Fixed
+- fixed bug that roundtrip statistics raises an exception when no data is available.
+- fixed possible exception that "_short_filter_names" does not exist
+- fixed missing namespace for IsReferenceParameter attribute
+ 
 ## [2.0.0a3] - 2023-06-08
 
 ### Added
 - SdcClient.start_all has optional parameter "check_get_service"
 - 
 ### Changed
 - moved port type name declaration from components.py to implementation classes [#176](https://github.com/Draegerwerk/sdc11073/issues/176)
```

### Comparing `sdc11073-2.0.0a3/docs/sdc_social_preview.jpg` & `sdc11073-2.0.0a4/docs/sdc_social_preview.jpg`

 * *Files identical despite different names*

### Comparing `sdc11073-2.0.0a3/src/sdc11073/certloader.py` & `sdc11073-2.0.0a4/src/sdc11073/certloader.py`

 * *Files identical despite different names*

### Comparing `sdc11073-2.0.0a3/src/sdc11073/commlog.py` & `sdc11073-2.0.0a4/src/sdc11073/commlog.py`

 * *Files identical despite different names*

### Comparing `sdc11073-2.0.0a3/src/sdc11073/definitions_base.py` & `sdc11073-2.0.0a4/src/sdc11073/definitions_base.py`

 * *Files identical despite different names*

### Comparing `sdc11073-2.0.0a3/src/sdc11073/definitions_sdc.py` & `sdc11073-2.0.0a4/src/sdc11073/definitions_sdc.py`

 * *Files identical despite different names*

### Comparing `sdc11073-2.0.0a3/src/sdc11073/etc.py` & `sdc11073-2.0.0a4/src/sdc11073/etc.py`

 * *Files identical despite different names*

### Comparing `sdc11073-2.0.0a3/src/sdc11073/exceptions.py` & `sdc11073-2.0.0a4/src/sdc11073/exceptions.py`

 * *Files identical despite different names*

### Comparing `sdc11073-2.0.0a3/src/sdc11073/location.py` & `sdc11073-2.0.0a4/src/sdc11073/location.py`

 * *Files identical despite different names*

### Comparing `sdc11073-2.0.0a3/src/sdc11073/loghelper.py` & `sdc11073-2.0.0a4/src/sdc11073/loghelper.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import logging
+from logging import handlers as logging_handlers
 import traceback
 
 
 # pylint: disable=invalid-name
 
 def ensure_log_stream():
     """Method makes sure that the sdc11073 root Logger has a stream handler with the default format.
@@ -38,15 +39,15 @@
 
 def basic_logging_setup(root_logger_name='sdc', level=logging.INFO, log_file_name=None):
     logging.basicConfig(format="%(asctime)s - %(name)s - %(levelname)s - %(message)s", level=level)
     reset_log_levels(root_logger_name)
     reset_handlers(root_logger_name)
     formatter = logging.Formatter("%(asctime)s - %(name)s - %(levelname)s - %(message)s")
     if log_file_name:
-        file_handler = logging.handlers.RotatingFileHandler(log_file_name,
+        file_handler = logging_handlers.RotatingFileHandler(log_file_name,
                                                             maxBytes=5000000,
                                                             backupCount=2)
         file_handler.setFormatter(formatter)
 
 
 class LoggerAdapter:
     """
```

### Comparing `sdc11073-2.0.0a3/src/sdc11073/multikey.py` & `sdc11073-2.0.0a4/src/sdc11073/multikey.py`

 * *Files identical despite different names*

### Comparing `sdc11073-2.0.0a3/src/sdc11073/namespaces.py` & `sdc11073-2.0.0a4/src/sdc11073/namespaces.py`

 * *Files identical despite different names*

### Comparing `sdc11073-2.0.0a3/src/sdc11073/schema_resolver.py` & `sdc11073-2.0.0a4/src/sdc11073/schema_resolver.py`

 * *Files identical despite different names*

### Comparing `sdc11073-2.0.0a3/src/sdc11073/dispatch/dispatchkey.py` & `sdc11073-2.0.0a4/src/sdc11073/dispatch/dispatchkey.py`

 * *Files identical despite different names*

### Comparing `sdc11073-2.0.0a3/src/sdc11073/dispatch/messageconverter.py` & `sdc11073-2.0.0a4/src/sdc11073/dispatch/messageconverter.py`

 * *Files identical despite different names*

### Comparing `sdc11073-2.0.0a3/src/sdc11073/dispatch/pathelementregistry.py` & `sdc11073-2.0.0a4/src/sdc11073/dispatch/pathelementregistry.py`

 * *Files identical despite different names*

### Comparing `sdc11073-2.0.0a3/src/sdc11073/dispatch/request.py` & `sdc11073-2.0.0a4/src/sdc11073/dispatch/request.py`

 * *Files identical despite different names*

### Comparing `sdc11073-2.0.0a3/src/sdc11073/httpserver/compression.py` & `sdc11073-2.0.0a4/src/sdc11073/httpserver/compression.py`

 * *Files identical despite different names*

### Comparing `sdc11073-2.0.0a3/src/sdc11073/httpserver/httpreader.py` & `sdc11073-2.0.0a4/src/sdc11073/httpserver/httpreader.py`

 * *Files identical despite different names*

### Comparing `sdc11073-2.0.0a3/src/sdc11073/httpserver/httprequesthandler.py` & `sdc11073-2.0.0a4/src/sdc11073/httpserver/httprequesthandler.py`

 * *Files identical despite different names*

### Comparing `sdc11073-2.0.0a3/src/sdc11073/httpserver/httpserverimpl.py` & `sdc11073-2.0.0a4/src/sdc11073/httpserver/httpserverimpl.py`

 * *Files identical despite different names*

### Comparing `sdc11073-2.0.0a3/src/sdc11073/mdib/clientmdib.py` & `sdc11073-2.0.0a4/src/sdc11073/mdib/clientmdib.py`

 * *Files identical despite different names*

### Comparing `sdc11073-2.0.0a3/src/sdc11073/mdib/clientmdibxtra.py` & `sdc11073-2.0.0a4/src/sdc11073/mdib/clientmdibxtra.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 import time
-from collections import namedtuple, deque
+from collections import deque
 from concurrent import futures
+from dataclasses import dataclass
 from statistics import mean, stdev
 from threading import Lock
 
-from .. import observableproperties as properties
-from ..exceptions import ApiUsageError
+from sdc11073 import observableproperties as properties
+from sdc11073.exceptions import ApiUsageError
 
 PROFILING = False
 if PROFILING:
     import cProfile
     import pstats
     from io import StringIO
 
@@ -20,53 +21,48 @@
 
 LOG_WF_AGE_INTERVAL = 30  # how often a log message is written with mean and stdev of waveforms age
 AGE_CALC_SAMPLES_COUNT = 100  # amount of data for wf mean age and stdev calculation
 
 
 class DeterminationTimeWarner:
     """A Helper to reduce log warnings regarding determination time."""
+
     ST_IN_RANGE = 0
     ST_OUT_OF_RANGE = 1
     result_lookup = {
-        # (last, current) :  (action, shall_repeat)
         (ST_IN_RANGE, ST_IN_RANGE): (A_NO_LOG, False),
         (ST_IN_RANGE, ST_OUT_OF_RANGE): (A_OUT_OF_RANGE, False),
         (ST_OUT_OF_RANGE, ST_OUT_OF_RANGE): (A_STILL_OUT_OF_RANGE, True),
-        (ST_OUT_OF_RANGE, ST_IN_RANGE): (A_BACK_IN_RANGE, False)
+        (ST_OUT_OF_RANGE, ST_IN_RANGE): (A_BACK_IN_RANGE, False),
     }
 
     def __init__(self, repeat_period=30):
         self.repeat_period = repeat_period
         self._last_log_time = 0
         self.last_state = self.ST_IN_RANGE
 
     def get_out_of_determination_time_log_state(self, min_age, max_age, warn_limit):
-        """
-        @return: one of above constants
-        """
+        """:return: one of above constants."""
         now = time.time()
-        if min_age < -warn_limit or max_age > warn_limit:
-            current_state = self.ST_OUT_OF_RANGE
-        else:
-            current_state = self.ST_IN_RANGE
+        current_state = self.ST_OUT_OF_RANGE if min_age < -warn_limit or max_age > warn_limit else self.ST_IN_RANGE
         action, shall_repeat = self.result_lookup[(self.last_state, current_state)]
         if self.last_state != current_state:
             # a state transition
             self.last_state = current_state
             self._last_log_time = now
             return action
         # no state transition, but might need repeated logging
         if shall_repeat and now - self._last_log_time >= self.repeat_period:
             self._last_log_time = now
             return action
         return A_NO_LOG
 
 
 class AgeLogger:
-    """A helper tht logs if incoming states are too old or in the future"""
+    """A helper tht logs if incoming states are too old or in the future."""
 
     def __init__(self, metric_time_warner, warn_limit, log_prefix, mdib_version):
         self._metric_time_warner = metric_time_warner
         self._warn_limit = warn_limit
         self._log_prefix = log_prefix
         self._mdib_version = mdib_version
         self.age_list = []
@@ -80,58 +76,66 @@
             return
         min_age = min(self.age_list)
         max_age = max(self.age_list)
 
         shall_log = self._metric_time_warner.get_out_of_determination_time_log_state(
             min_age, max_age, self._warn_limit)
         if shall_log == A_OUT_OF_RANGE:
-            logger.warn(
+            logger.warning(
                 '{} mdib_version {}: age of states outside limit of {} sec.: max, min = {:03f}, {:03f}',
                 self._log_prefix, self._mdib_version, self._warn_limit, max_age, min_age)
         elif shall_log == A_STILL_OUT_OF_RANGE:
-            logger.warn(
+            logger.warning(
                 '{} mdib_version {}: age of states still outside limit of {} sec.: max, min = {:03f}, {:03f}',
                 self._log_prefix, self._mdib_version, self._warn_limit, max_age, min_age)
         elif shall_log == A_BACK_IN_RANGE:
             logger.info(
                 '{} mdib_version {}: age of states back in limit of {} sec.: max, min = {:03f}, {:03f}',
                 self._log_prefix, self._mdib_version, self._warn_limit, max_age, min_age)
 
 
-_AgeData = namedtuple('_AgeData', 'mean_age stdev min_age max_age')
+@dataclass
+class AgeData:
+    """Container for some statistical age data."""
+
+    mean_age: float
+    stdev: float
+    min_age: float
+    max_age: float
 
 
 class AgeStatistics:
-    """Keep age data of a single state over time. """
+    """Keep age data of a single state over time."""
 
     def __init__(self, entry_count=None):
         length = entry_count or AGE_CALC_SAMPLES_COUNT
         self._age_of_data_list = deque(
             maxlen=length)  # used to calculate average age of samples when received
         self._lock = Lock()
 
     def process_state(self, state):
         try:
             age = time.time() - state.MetricValue.DeterminationTime
             with self._lock:
                 self._age_of_data_list.append(age)
-        except AttributeError:
+        except AttributeError as ex:
             if not state.is_metric_state:
-                raise ApiUsageError(f'{self.__class__.__name__} can only handle metric states')
+                raise ApiUsageError(f'{self.__class__.__name__} can only handle metric states') from ex
             # or state.MetricValue is None or  DeterminationTime is None: ignore this
 
-    def get_age_stdev(self) -> _AgeData:
+    def get_age_stdev(self) -> AgeData:
+        """Calculate age statistics data."""
         if len(self._age_of_data_list) < 3:
-            return _AgeData(0, 0, 0, 0)
+            return AgeData(0.0, 0.0, 0.0, 0.0)
         with self._lock:
             min_value = min(self._age_of_data_list)
             max_value = max(self._age_of_data_list)
             mean_data = mean(self._age_of_data_list)
             std_deviation = stdev(self._age_of_data_list)
-            return _AgeData(mean_data, std_deviation, min_value, max_value)
+            return AgeData(mean_data, std_deviation, min_value, max_value)
 
 
 class ClientMdibMethods:
     DETERMINATIONTIME_WARN_LIMIT = 1.0  # in seconds
 
     def __init__(self, client_mdib, logger):
         self._mdib = client_mdib
@@ -146,23 +150,23 @@
         self._age_statistics = {}
         self._calculate_wf_age_stats = False
 
     def set_calculate_wf_age_stats(self, shall_calculate: bool):
         self._calculate_wf_age_stats = shall_calculate
 
     def wait_metric_matches(self, handle, matches_func, timeout):
-        """ wait until a matching metric has been received. The matching is defined by the handle of the metric
+        """Wait until a matching metric has been received. The matching is defined by the handle of the metric
         and the result of a matching function. If the matching function returns true, this function returns.
         :param handle: The handle string of the metric of interest.
         :param matches_func: a callable, argument is the current state with matching handle. Can be None, in that case every state matches
         Example:
             expected = 42
             def isMatchingValue(state):
                 if state.MetricValue is None:
-                    return False
+                    return False.
 
                 found_value = state.MetricValue.Value
                 return [expected] == found_value
         :param timeout: timeout in seconds
         @return: the matching state. In case of a timeout it raises a TimeoutError exception.
         """
         fut = futures.Future()
@@ -180,16 +184,16 @@
             ret = fut.result(timeout)
             self._logger.debug('wait_metric_matches: got result after {:.2f} seconds', time.monotonic() - begin)
             return ret
         finally:
             properties.unbind(self._mdib, metrics_by_handle=on_metrics_by_handle)
 
     def mk_proposed_state(self, descriptor_handle, copy_current_state=True, handle=None):
-        """ Create a new state that can be used as proposed state in according operations.
-        The new state is not part of mdib!
+        """Create a new state that can be used as proposed state in according operations.
+        The new state is not part of mdib!.
 
         :param descriptor_handle: the descriptor
         :param copy_current_state: if True, all members of existing state will be copied to new state
         :param handle: if this is a multi state class, then this is the handle of the existing state that shall be used for copy.
         :return:
         """
         descr = self._mdib.descriptions.handle.get_one(descriptor_handle)
@@ -203,18 +207,18 @@
             else:
                 old_state = lookup.descriptorHandle.get_one(descriptor_handle)
             new_state.update_from_other_container(old_state)
         return new_state
 
     def sync_context_states(self):
         """This method requests all context states from device and deletes all local context states that are not
-        available in response from Device."""
+        available in response from Device.
+        """
         self._logger.info('_sync_context_states called')
         context_service = self._sdc_client.client('Context')
-        # mdib_version, sequence_id, context_state_containers = context_service.get_context_states()
         response = context_service.get_context_states()
         context_state_containers = response.result.ContextState
 
         devices_context_state_handles = [s.Handle for s in context_state_containers]
         with self._mdib.context_states.lock:
             for obj in self._mdib.context_states.objects:
                 if obj.Handle not in devices_context_state_handles:
@@ -255,15 +259,15 @@
                     if state_container.ActivationState == model.pm_types.ComponentActivation.ON and \
                             state_container.MetricValue.MetricQuality.Validity not in [
                         model.pm_types.MeasurementValidity.INVALID,
                         model.pm_types.MeasurementValidity.NA,
                         model.pm_types.MeasurementValidity.MEASUREMENT_ONGOING]:
                         determination_time = state_container.MetricValue.DeterminationTime
                         if determination_time is None:
-                            self._logger.warn(
+                            self._logger.warning(
                                 'EpisodicMetricReport: metric {} version {} has no DeterminationTime',
                                 desc_h, state_container.StateVersion)
                         else:
                             age_logger.add_determination_time(determination_time)
 
         age_logger.log_age_warnings(self._logger)
 
@@ -312,70 +316,78 @@
                 min_age = min(waveform_age.values())
                 max_age = max(waveform_age.values())
                 shall_log = self.waveform_time_warner.get_out_of_determination_time_log_state(
                     min_age, max_age, self.DETERMINATIONTIME_WARN_LIMIT)
                 if shall_log != A_NO_LOG:
                     tmp = ', '.join(f'"{k}": {v:.3f}sec.' for k, v in waveform_age.items())
                     if shall_log == A_OUT_OF_RANGE:
-                        self._logger.warn(
+                        self._logger.warning(
                             '_on_waveform_report mdib_version {}: age of samples outside limit of {} sec.: {}',
                             self._mdib.mdib_version, self.DETERMINATIONTIME_WARN_LIMIT, tmp)
                     elif shall_log == A_STILL_OUT_OF_RANGE:
-                        self._logger.warn(
+                        self._logger.warning(
                             '_on_waveform_report mdib_version {}: age of samples still outside limit of {} sec.: {}',
                             self._mdib.mdib_version, self.DETERMINATIONTIME_WARN_LIMIT, tmp)
                     elif shall_log == A_BACK_IN_RANGE:
                         self._logger.info(
                             '_on_waveform_report mdib_version {}: age of samples back in limit of {} sec.: {}',
                             self._mdib.mdib_version, self.DETERMINATIONTIME_WARN_LIMIT, tmp)
             if LOG_WF_AGE_INTERVAL:
                 now = time.time()
                 if now - self._last_wf_age_log >= LOG_WF_AGE_INTERVAL:
                     age_data = self.get_wf_age_stdev()
-                    self._logger.info('waveform mean age={:.1f}ms., stdev={:.2f}ms. min={:.1f}ms., max={}',
-                                      age_data.mean_age * 1000., age_data.stdev * 1000.,
-                                      age_data.min_age * 1000., age_data.max_age * 1000.)
+                    if age_data is not None:
+                        self._logger.info('waveform mean age={:.1f}ms., stdev={:.2f}ms. min={:.1f}ms., max={}',
+                                          age_data.mean_age * 1000., age_data.stdev * 1000.,
+                                          age_data.min_age * 1000., age_data.max_age * 1000.)
                     self._last_wf_age_log = now
 
     def _on_episodic_context_report(self, received_message_data):
         cls = self._mdib.data_model.msg_types.EpisodicContextReport
         report = cls.from_node(received_message_data.p_msg.msg_node)
         self._mdib.process_incoming_context_states_report(received_message_data.mdib_version_group, report)
 
     def _on_episodic_component_report(self, received_message_data):
         """The EpisodicComponentReport is sent if at least one property of at least one component state has changed
         and SHOULD contain only the changed component states.
-        Components are MDSs, VMDs, Channels. Not metrics and alarms
+        Components are MDSs, VMDs, Channels. Not metrics and alarms.
         """
         cls = self._mdib.data_model.msg_types.EpisodicComponentReport
         report = cls.from_node(received_message_data.p_msg.msg_node)
         self._mdib.process_incoming_component_states_report(received_message_data.mdib_version_group, report)
 
     def _on_description_modification_report(self, received_message_data):
         """The EpisodicComponentReport is sent if at least one property of at least one component state has changed
         and SHOULD contain only the changed component states.
-        Components are MDSs, VMDs, Channels. Not metrics and alarms
+        Components are MDSs, VMDs, Channels. Not metrics and alarms.
         """
         cls = self._mdib.data_model.msg_types.DescriptionModificationReport
         report = cls.from_node(received_message_data.p_msg.msg_node)
         self._mdib.process_incoming_description_modifications(received_message_data.mdib_version_group, report)
 
     def _process_age_statistics(self, state_containers):
         for st in state_containers:
             age_stat = self._age_statistics.get(st.DescriptorHandle)
             if age_stat is None:
                 age_stat = AgeStatistics()
                 self._age_statistics[st.DescriptorHandle] = age_stat
             age_stat.process_state(st)
 
-    def get_wf_age_stdev(self):
+    def get_wf_age_stdev(self) -> AgeData:
+        """Create some statistics data for age of waveform data when it arrived.
+
+        Data is used for logging.
+        """
+        if len(self._age_statistics) < 3:
+            return AgeData(0.0, 0.0, 0.0, 0.0)
+
         means = []
         stdevs = []
         mins = []
         maxs = []
         for age_stat in self._age_statistics.values():
             age_data = age_stat.get_age_stdev()
             means.append(age_data.mean_age)
             stdevs.append(age_data.stdev)
             mins.append(age_data.min_age)
             maxs.append(age_data.max_age)
-        return _AgeData(mean(means), mean(stdevs), min(mins), max(maxs))
+        return AgeData(mean(means), mean(stdevs), min(mins), max(maxs))
```

### Comparing `sdc11073-2.0.0a3/src/sdc11073/mdib/containerbase.py` & `sdc11073-2.0.0a4/src/sdc11073/mdib/containerbase.py`

 * *Files identical despite different names*

### Comparing `sdc11073-2.0.0a3/src/sdc11073/mdib/descriptorcontainers.py` & `sdc11073-2.0.0a4/src/sdc11073/mdib/descriptorcontainers.py`

 * *Files identical despite different names*

### Comparing `sdc11073-2.0.0a3/src/sdc11073/mdib/devicemdib.py` & `sdc11073-2.0.0a4/src/sdc11073/mdib/devicemdib.py`

 * *Files identical despite different names*

### Comparing `sdc11073-2.0.0a3/src/sdc11073/mdib/devicemdibxtra.py` & `sdc11073-2.0.0a4/src/sdc11073/mdib/devicemdibxtra.py`

 * *Files identical despite different names*

### Comparing `sdc11073-2.0.0a3/src/sdc11073/mdib/devicewaveform.py` & `sdc11073-2.0.0a4/src/sdc11073/mdib/devicewaveform.py`

 * *Files identical despite different names*

### Comparing `sdc11073-2.0.0a3/src/sdc11073/mdib/mdibbase.py` & `sdc11073-2.0.0a4/src/sdc11073/mdib/mdibbase.py`

 * *Files identical despite different names*

### Comparing `sdc11073-2.0.0a3/src/sdc11073/mdib/statecontainers.py` & `sdc11073-2.0.0a4/src/sdc11073/mdib/statecontainers.py`

 * *Files identical despite different names*

### Comparing `sdc11073-2.0.0a3/src/sdc11073/mdib/transactions.py` & `sdc11073-2.0.0a4/src/sdc11073/mdib/transactions.py`

 * *Files identical despite different names*

### Comparing `sdc11073-2.0.0a3/src/sdc11073/netconn/__init__.py` & `sdc11073-2.0.0a4/src/sdc11073/netconn/__init__.py`

 * *Files identical despite different names*

### Comparing `sdc11073-2.0.0a3/src/sdc11073/observableproperties/observables.py` & `sdc11073-2.0.0a4/src/sdc11073/observableproperties/observables.py`

 * *Files identical despite different names*

### Comparing `sdc11073-2.0.0a3/src/sdc11073/observableproperties/valuecollector.py` & `sdc11073-2.0.0a4/src/sdc11073/observableproperties/valuecollector.py`

 * *Files identical despite different names*

### Comparing `sdc11073-2.0.0a3/src/sdc11073/pysoap/msgfactory.py` & `sdc11073-2.0.0a4/src/sdc11073/pysoap/msgfactory.py`

 * *Files identical despite different names*

### Comparing `sdc11073-2.0.0a3/src/sdc11073/pysoap/msgreader.py` & `sdc11073-2.0.0a4/src/sdc11073/pysoap/msgreader.py`

 * *Files identical despite different names*

### Comparing `sdc11073-2.0.0a3/src/sdc11073/pysoap/soapclient.py` & `sdc11073-2.0.0a4/src/sdc11073/pysoap/soapclient.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 Using lxml based SoapEnvelope."""
 from __future__ import annotations
 
 import socket
 import sys
 import time
 import traceback
+from lxml.etree import XMLSyntaxError
 from http.client import CannotSendRequest, BadStatusLine, NotConnected, UnknownTransferEncoding
 from http.client import HTTPConnection, HTTPSConnection
 from http.client import HTTPException, HTTPResponse
 from threading import Lock
 from typing import List, Optional, TYPE_CHECKING, Union
 
 from .. import commlog
@@ -294,17 +295,21 @@
 
             content = HTTPReader.read_response_body(response)
 
             if response.status >= 300:
                 self._log.error(
                     "{}: POST to netloc='{}' path='{}': could not send request, HTTP response={}\ncontent='{}'", msg,
                     self._netloc, path, response.status, content.decode('utf-8'))
-                tmp = self._msg_reader.read_received_message(content)
-                soap_fault = Fault.from_node(tmp.p_msg.msg_node)
-                raise HTTPReturnCodeError(response.status, response.reason, soap_fault)
+                try:
+                    tmp = self._msg_reader.read_received_message(content)
+                except XMLSyntaxError as ex:
+                    raise HTTPReturnCodeError(response.status, response.reason, None) from ex
+                else:
+                    soap_fault = Fault.from_node(tmp.p_msg.msg_node)
+                    raise HTTPReturnCodeError(response.status, response.reason, soap_fault)
 
             response_headers = {k.lower(): v for k, v in response.getheaders()}
 
             self._log.debug('{}: response:{}; content has {} Bytes ', msg, response_headers, len(content))
             commlog.get_communication_logger().log_soap_response_in(content, 'POST')
             return response, content
```

### Comparing `sdc11073-2.0.0a3/src/sdc11073/pysoap/soapclient_async.py` & `sdc11073-2.0.0a4/src/sdc11073/pysoap/soapclient_async.py`

 * *Files identical despite different names*

### Comparing `sdc11073-2.0.0a3/src/sdc11073/pysoap/soapclientpool.py` & `sdc11073-2.0.0a4/src/sdc11073/pysoap/soapclientpool.py`

 * *Files identical despite different names*

### Comparing `sdc11073-2.0.0a3/src/sdc11073/pysoap/soapenvelope.py` & `sdc11073-2.0.0a4/src/sdc11073/pysoap/soapenvelope.py`

 * *Files identical despite different names*

### Comparing `sdc11073-2.0.0a3/src/sdc11073/roles/alarmprovider.py` & `sdc11073-2.0.0a4/src/sdc11073/roles/alarmprovider.py`

 * *Files 1% similar despite different names*

```diff
@@ -351,15 +351,14 @@
 
     def _run_worker_job(self):
         self._update_alert_system_state_current_alerts()
 
     def _update_alert_system_state_current_alerts(self):
         """ updates AlertSystemState present alarms list"""
         states_needing_update = self._get_alert_system_states_needing_update()
-        self._logger.debug(f'{len(states_needing_update)} states_needing_update')
         if len(states_needing_update) > 0:
             try:
                 with self._mdib.transaction_manager() as mgr:
                     tr_states = [mgr.get_state(s.DescriptorHandle) for s in states_needing_update]
                     self._update_alert_system_states(self._mdib, mgr, tr_states)
             except Exception:
                 exc = traceback.format_exc()
```

### Comparing `sdc11073-2.0.0a3/src/sdc11073/roles/audiopauseprovider.py` & `sdc11073-2.0.0a4/src/sdc11073/roles/audiopauseprovider.py`

 * *Files identical despite different names*

### Comparing `sdc11073-2.0.0a3/src/sdc11073/roles/clockprovider.py` & `sdc11073-2.0.0a4/src/sdc11073/roles/clockprovider.py`

 * *Files identical despite different names*

### Comparing `sdc11073-2.0.0a3/src/sdc11073/roles/contextprovider.py` & `sdc11073-2.0.0a4/src/sdc11073/roles/contextprovider.py`

 * *Files identical despite different names*

### Comparing `sdc11073-2.0.0a3/src/sdc11073/roles/metricprovider.py` & `sdc11073-2.0.0a4/src/sdc11073/roles/metricprovider.py`

 * *Files identical despite different names*

### Comparing `sdc11073-2.0.0a3/src/sdc11073/roles/nomenclature.py` & `sdc11073-2.0.0a4/src/sdc11073/roles/nomenclature.py`

 * *Files identical despite different names*

### Comparing `sdc11073-2.0.0a3/src/sdc11073/roles/patientcontextprovider.py` & `sdc11073-2.0.0a4/src/sdc11073/roles/patientcontextprovider.py`

 * *Files identical despite different names*

### Comparing `sdc11073-2.0.0a3/src/sdc11073/roles/product.py` & `sdc11073-2.0.0a4/src/sdc11073/roles/product.py`

 * *Files identical despite different names*

### Comparing `sdc11073-2.0.0a3/src/sdc11073/roles/providerbase.py` & `sdc11073-2.0.0a4/src/sdc11073/roles/providerbase.py`

 * *Files identical despite different names*

### Comparing `sdc11073-2.0.0a3/src/sdc11073/sdcclient/components.py` & `sdc11073-2.0.0a4/src/sdc11073/sdcclient/components.py`

 * *Files identical despite different names*

### Comparing `sdc11073-2.0.0a3/src/sdc11073/sdcclient/manipulator.py` & `sdc11073-2.0.0a4/src/sdc11073/sdcclient/manipulator.py`

 * *Files identical despite different names*

### Comparing `sdc11073-2.0.0a3/src/sdc11073/sdcclient/operations.py` & `sdc11073-2.0.0a4/src/sdc11073/sdcclient/operations.py`

 * *Files identical despite different names*

### Comparing `sdc11073-2.0.0a3/src/sdc11073/sdcclient/request_handler_deferred.py` & `sdc11073-2.0.0a4/src/sdc11073/sdcclient/request_handler_deferred.py`

 * *Files identical despite different names*

### Comparing `sdc11073-2.0.0a3/src/sdc11073/sdcclient/sdcclientimpl.py` & `sdc11073-2.0.0a4/src/sdc11073/sdcclient/sdcclientimpl.py`

 * *Files 0% similar despite different names*

```diff
@@ -660,15 +660,15 @@
         :param ssl_context: a ssl context or None
         :param validate: bool
         :param log_prefix: a string
         :param default_components: a SdcClientComponents instance or None
         :param specific_components: a SdcClientComponents instance or None
         :return:
         """
-        device_locations = wsd_service.get_x_addrs()
+        device_locations = wsd_service.x_addrs
         if not device_locations:
             raise RuntimeError(f'discovered Service has no address!{wsd_service}')
         device_location = device_locations[0]
         for sdc_definition in ProtocolsRegistry.protocols:
             if sdc_definition.types_match(wsd_service.types):
                 return cls(device_location, sdc_definition, ssl_context, validate=validate, log_prefix=log_prefix,
                            default_components=default_components, specific_components=specific_components)
```

### Comparing `sdc11073-2.0.0a3/src/sdc11073/sdcclient/subscription.py` & `sdc11073-2.0.0a4/src/sdc11073/sdcclient/subscription.py`

 * *Files identical despite different names*

### Comparing `sdc11073-2.0.0a3/src/sdc11073/sdcclient/serviceclients/containmenttreeservice.py` & `sdc11073-2.0.0a4/src/sdc11073/sdcclient/serviceclients/containmenttreeservice.py`

 * *Files identical despite different names*

### Comparing `sdc11073-2.0.0a3/src/sdc11073/sdcclient/serviceclients/contextservice.py` & `sdc11073-2.0.0a4/src/sdc11073/sdcclient/serviceclients/contextservice.py`

 * *Files identical despite different names*

### Comparing `sdc11073-2.0.0a3/src/sdc11073/sdcclient/serviceclients/getservice.py` & `sdc11073-2.0.0a4/src/sdc11073/sdcclient/serviceclients/getservice.py`

 * *Files identical despite different names*

### Comparing `sdc11073-2.0.0a3/src/sdc11073/sdcclient/serviceclients/localizationservice.py` & `sdc11073-2.0.0a4/src/sdc11073/sdcclient/serviceclients/localizationservice.py`

 * *Files identical despite different names*

### Comparing `sdc11073-2.0.0a3/src/sdc11073/sdcclient/serviceclients/serviceclientbase.py` & `sdc11073-2.0.0a4/src/sdc11073/sdcclient/serviceclients/serviceclientbase.py`

 * *Files identical despite different names*

### Comparing `sdc11073-2.0.0a3/src/sdc11073/sdcclient/serviceclients/setservice.py` & `sdc11073-2.0.0a4/src/sdc11073/sdcclient/serviceclients/setservice.py`

 * *Files identical despite different names*

### Comparing `sdc11073-2.0.0a3/src/sdc11073/sdcclient/serviceclients/stateeventservice.py` & `sdc11073-2.0.0a4/src/sdc11073/sdcclient/serviceclients/stateeventservice.py`

 * *Files identical despite different names*

### Comparing `sdc11073-2.0.0a3/src/sdc11073/sdcdevice/components.py` & `sdc11073-2.0.0a4/src/sdc11073/sdcdevice/components.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from __future__ import annotations
 
 import copy
 from dataclasses import dataclass
-from typing import Type, Callable, Any, TYPE_CHECKING
+from typing import Callable, Any, TYPE_CHECKING
 
 from .operations import get_operation_class
 from .porttypes.containmenttreeserviceimpl import ContainmentTreeService
 from .porttypes.contextserviceimpl import ContextService
 from .porttypes.descriptioneventserviceimpl import DescriptionEventService
 from .porttypes.getserviceimpl import GetService
 from .porttypes.localizationservice import LocalizationService
@@ -37,23 +37,23 @@
 
 # pylint: enable=cyclic-import
 
 
 # Dependency injection: This class defines which component implementations the sdc device will use.
 @dataclass()
 class SdcDeviceComponents:
-    soap_client_class: Type[Any] = None
-    msg_factory_class: Type[MessageFactory] = None
-    msg_reader_class: Type[MessageReader] = None
-    client_msg_reader_class: Type[MessageReader] = None  # the corresponding reader for client
-    xml_reader_class: Type[MessageReader] = None  # needed to read xml based mdib files
+    soap_client_class: type[Any] = None
+    msg_factory_class: type[MessageFactory] = None
+    msg_reader_class: type[MessageReader] = None
+    client_msg_reader_class: type[MessageReader] = None  # the corresponding reader for client
+    xml_reader_class: type[MessageReader] = None  # needed to read xml based mdib files
     services_factory: Callable[[Any, dict, Any], HostedServices] = None
     operation_cls_getter: Callable[[QName], type] = None
-    sco_operations_registry_class: Type[AbstractScoOperationsRegistry] = None
-    subscriptions_manager_class: dict[str, SubscriptionManagerProtocol] = None
+    sco_operations_registry_class: type[AbstractScoOperationsRegistry] = None
+    subscriptions_manager_class: dict[str, type[SubscriptionManagerProtocol]] = None
     role_provider_class: type = None
     scopes_factory: Callable[[DeviceMdibContainer], ScopesType] = None
     hosted_services: dict = None
 
     def merge(self, other):
         def _merge(attr_name):
             other_value = getattr(other, attr_name)
@@ -61,15 +61,14 @@
                 setattr(self, attr_name, other_value)
 
         _merge('msg_factory_class')
         _merge('msg_reader_class')
         _merge('services_factory')
         _merge('operation_cls_getter')
         _merge('sco_operations_registry_class')
-        # _merge('subscriptions_manager_class')
         _merge('role_provider_class')
         _merge('scopes_factory')
         if other.hosted_services is not None:
             self.hosted_services = other.hosted_services
         if other.subscriptions_manager_class is not None:
             for key, value in other.subscriptions_manager_class.items():
                 self.subscriptions_manager_class[key] = value
```

### Comparing `sdc11073-2.0.0a3/src/sdc11073/sdcdevice/dpwshostedservice.py` & `sdc11073-2.0.0a4/src/sdc11073/sdcdevice/dpwshostedservice.py`

 * *Files identical despite different names*

### Comparing `sdc11073-2.0.0a3/src/sdc11073/sdcdevice/intervaltimer.py` & `sdc11073-2.0.0a4/src/sdc11073/sdcdevice/intervaltimer.py`

 * *Files identical despite different names*

### Comparing `sdc11073-2.0.0a3/src/sdc11073/sdcdevice/operations.py` & `sdc11073-2.0.0a4/src/sdc11073/sdcdevice/operations.py`

 * *Files identical despite different names*

### Comparing `sdc11073-2.0.0a3/src/sdc11073/sdcdevice/periodicreports.py` & `sdc11073-2.0.0a4/src/sdc11073/sdcdevice/periodicreports.py`

 * *Files identical despite different names*

### Comparing `sdc11073-2.0.0a3/src/sdc11073/sdcdevice/sco.py` & `sdc11073-2.0.0a4/src/sdc11073/sdcdevice/sco.py`

 * *Files identical despite different names*

### Comparing `sdc11073-2.0.0a3/src/sdc11073/sdcdevice/scopesfactory.py` & `sdc11073-2.0.0a4/src/sdc11073/sdcdevice/scopesfactory.py`

 * *Files identical despite different names*

### Comparing `sdc11073-2.0.0a3/src/sdc11073/sdcdevice/sdcdeviceimpl.py` & `sdc11073-2.0.0a4/src/sdc11073/sdcdevice/sdcdeviceimpl.py`

 * *Files identical despite different names*

### Comparing `sdc11073-2.0.0a3/src/sdc11073/sdcdevice/servicesfactory.py` & `sdc11073-2.0.0a4/src/sdc11073/sdcdevice/servicesfactory.py`

 * *Files identical despite different names*

### Comparing `sdc11073-2.0.0a3/src/sdc11073/sdcdevice/subscriptionmgr.py` & `sdc11073-2.0.0a4/src/sdc11073/sdcdevice/subscriptionmgr.py`

 * *Files identical despite different names*

### Comparing `sdc11073-2.0.0a3/src/sdc11073/sdcdevice/subscriptionmgr_async.py` & `sdc11073-2.0.0a4/src/sdc11073/sdcdevice/subscriptionmgr_async.py`

 * *Files identical despite different names*

### Comparing `sdc11073-2.0.0a3/src/sdc11073/sdcdevice/subscriptionmgr_base.py` & `sdc11073-2.0.0a4/src/sdc11073/sdcdevice/subscriptionmgr_base.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -243,18 +243,18 @@
 
 
 class ActionBasedSubscription(SubscriptionBase):
     """Subscription for specific actions.
     Actions are a space separated list of strings in FilterType.text. """
 
     def __init__(self, *args, **kwargs):
-        super().__init__(*args, **kwargs)
         # split the filter sting into separate action strings and keep them
         self.actions_filter: list[str] = []
         self._short_filter_names: list[str] = [] # helper for shorter log entries
+        super().__init__(*args, **kwargs)
         if self.filter_type is not None:
             self.actions_filter.extend(self.filter_type.text.split())
             self._short_filter_names = [f.split('/')[-1] for f in self.actions_filter]
 
     def matches(self, what: Any) -> bool:
         """
```

### Comparing `sdc11073-2.0.0a3/src/sdc11073/sdcdevice/waveforms.py` & `sdc11073-2.0.0a4/src/sdc11073/sdcdevice/waveforms.py`

 * *Files identical despite different names*

### Comparing `sdc11073-2.0.0a3/src/sdc11073/sdcdevice/porttypes/containmenttreeserviceimpl.py` & `sdc11073-2.0.0a4/src/sdc11073/sdcdevice/porttypes/containmenttreeserviceimpl.py`

 * *Files identical despite different names*

### Comparing `sdc11073-2.0.0a3/src/sdc11073/sdcdevice/porttypes/contextserviceimpl.py` & `sdc11073-2.0.0a4/src/sdc11073/sdcdevice/porttypes/contextserviceimpl.py`

 * *Files identical despite different names*

### Comparing `sdc11073-2.0.0a3/src/sdc11073/sdcdevice/porttypes/descriptioneventserviceimpl.py` & `sdc11073-2.0.0a4/src/sdc11073/sdcdevice/porttypes/descriptioneventserviceimpl.py`

 * *Files identical despite different names*

### Comparing `sdc11073-2.0.0a3/src/sdc11073/sdcdevice/porttypes/getserviceimpl.py` & `sdc11073-2.0.0a4/src/sdc11073/sdcdevice/porttypes/getserviceimpl.py`

 * *Files identical despite different names*

### Comparing `sdc11073-2.0.0a3/src/sdc11073/sdcdevice/porttypes/localizationservice.py` & `sdc11073-2.0.0a4/src/sdc11073/sdcdevice/porttypes/localizationservice.py`

 * *Files identical despite different names*

### Comparing `sdc11073-2.0.0a3/src/sdc11073/sdcdevice/porttypes/porttypebase.py` & `sdc11073-2.0.0a4/src/sdc11073/sdcdevice/porttypes/porttypebase.py`

 * *Files identical despite different names*

### Comparing `sdc11073-2.0.0a3/src/sdc11073/sdcdevice/porttypes/setserviceimpl.py` & `sdc11073-2.0.0a4/src/sdc11073/sdcdevice/porttypes/setserviceimpl.py`

 * *Files identical despite different names*

### Comparing `sdc11073-2.0.0a3/src/sdc11073/sdcdevice/porttypes/stateeventserviceimpl.py` & `sdc11073-2.0.0a4/src/sdc11073/sdcdevice/porttypes/stateeventserviceimpl.py`

 * *Files identical despite different names*

### Comparing `sdc11073-2.0.0a3/src/sdc11073/sdcdevice/porttypes/waveformserviceimpl.py` & `sdc11073-2.0.0a4/src/sdc11073/sdcdevice/porttypes/waveformserviceimpl.py`

 * *Files identical despite different names*

### Comparing `sdc11073-2.0.0a3/src/sdc11073/xml_types/actions.py` & `sdc11073-2.0.0a4/src/sdc11073/xml_types/actions.py`

 * *Files identical despite different names*

### Comparing `sdc11073-2.0.0a3/src/sdc11073/xml_types/addressing_types.py` & `sdc11073-2.0.0a4/src/sdc11073/xml_types/addressing_types.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 from __future__ import annotations
 
 import copy
 import uuid
 from typing import Optional, List, TYPE_CHECKING
-
 from sdc11073.namespaces import default_ns_helper as nsh
 from . import xml_structure as struct
 from .basetypes import XMLTypeBase, ElementWithText
 
 if TYPE_CHECKING:
     from lxml.etree import QName, Element
 
+_is_reference_parameter = nsh.WSA.tag('IsReferenceParameter')
 
 class EndpointReferenceType(XMLTypeBase):
     Address = struct.NodeStringProperty(nsh.WSA.tag('Address'))
     ReferenceParameters = struct.AnyEtreeNodeListProperty(nsh.WSA.tag('ReferenceParameters'), is_optional=True)
     PortType = struct.NodeTextQNameProperty(nsh.WSA.tag('PortType'), is_optional=True)
     _props = ['Address', 'ReferenceParameters', 'PortType']
 
@@ -92,22 +92,22 @@
         return reply_address
 
     def as_etree_node(self, q_name, ns_map):
         """ special handling of reference parameters"""
         node = super().as_etree_node(q_name, ns_map)
         for param in self.reference_parameters:
             tmp = copy.deepcopy(param)
-            tmp.set('IsReferenceParameter', 'true')
+            tmp.set(_is_reference_parameter, 'true')
             node.append(tmp)
         return node
 
     @classmethod
     def from_node(cls, node):
         """ special handling of reference parameters"""
         obj = cls()
         obj.update_from_node(node)
         # collect reference parameter child nodes
         for child in node:
-            is_reference_parameter = child.attrib.get('IsReferenceParameter', 'false')
+            is_reference_parameter = child.attrib.get(_is_reference_parameter, 'false')
             if is_reference_parameter.lower() == 'true':
                 obj.reference_parameters.append(child)
         return obj
```

### Comparing `sdc11073-2.0.0a3/src/sdc11073/xml_types/basetypes.py` & `sdc11073-2.0.0a4/src/sdc11073/xml_types/basetypes.py`

 * *Files identical despite different names*

### Comparing `sdc11073-2.0.0a3/src/sdc11073/xml_types/dataconverters.py` & `sdc11073-2.0.0a4/src/sdc11073/xml_types/dataconverters.py`

 * *Files identical despite different names*

### Comparing `sdc11073-2.0.0a3/src/sdc11073/xml_types/dpws_types.py` & `sdc11073-2.0.0a4/src/sdc11073/xml_types/dpws_types.py`

 * *Files identical despite different names*

### Comparing `sdc11073-2.0.0a3/src/sdc11073/xml_types/eventing_types.py` & `sdc11073-2.0.0a4/src/sdc11073/xml_types/eventing_types.py`

 * *Files identical despite different names*

### Comparing `sdc11073-2.0.0a3/src/sdc11073/xml_types/isoduration.py` & `sdc11073-2.0.0a4/src/sdc11073/xml_types/isoduration.py`

 * *Files identical despite different names*

### Comparing `sdc11073-2.0.0a3/src/sdc11073/xml_types/mex_types.py` & `sdc11073-2.0.0a4/src/sdc11073/xml_types/mex_types.py`

 * *Files identical despite different names*

### Comparing `sdc11073-2.0.0a3/src/sdc11073/xml_types/msg_qnames.py` & `sdc11073-2.0.0a4/src/sdc11073/xml_types/msg_qnames.py`

 * *Files identical despite different names*

### Comparing `sdc11073-2.0.0a3/src/sdc11073/xml_types/msg_types.py` & `sdc11073-2.0.0a4/src/sdc11073/xml_types/msg_types.py`

 * *Files identical despite different names*

### Comparing `sdc11073-2.0.0a3/src/sdc11073/xml_types/pm_qnames.py` & `sdc11073-2.0.0a4/src/sdc11073/xml_types/pm_qnames.py`

 * *Files identical despite different names*

### Comparing `sdc11073-2.0.0a3/src/sdc11073/xml_types/pm_types.py` & `sdc11073-2.0.0a4/src/sdc11073/xml_types/pm_types.py`

 * *Files identical despite different names*

### Comparing `sdc11073-2.0.0a3/src/sdc11073/xml_types/wsd_types.py` & `sdc11073-2.0.0a4/src/sdc11073/xml_types/wsd_types.py`

 * *Files identical despite different names*

### Comparing `sdc11073-2.0.0a3/src/sdc11073/xml_types/xml_structure.py` & `sdc11073-2.0.0a4/src/sdc11073/xml_types/xml_structure.py`

 * *Files identical despite different names*

### Comparing `sdc11073-2.0.0a3/src/sdc11073/xsd/BICEPS_MessageModel.xsd` & `sdc11073-2.0.0a4/src/sdc11073/xsd/BICEPS_MessageModel.xsd`

 * *Files identical despite different names*

### Comparing `sdc11073-2.0.0a3/src/sdc11073/xsd/BICEPS_ParticipantModel.xsd` & `sdc11073-2.0.0a4/src/sdc11073/xsd/BICEPS_ParticipantModel.xsd`

 * *Files identical despite different names*

### Comparing `sdc11073-2.0.0a3/src/sdc11073/xsd/ExtensionPoint.xsd` & `sdc11073-2.0.0a4/src/sdc11073/xsd/ExtensionPoint.xsd`

 * *Files identical despite different names*

### Comparing `sdc11073-2.0.0a3/src/sdc11073/xsd/MetadataExchange.xsd` & `sdc11073-2.0.0a4/src/sdc11073/xsd/MetadataExchange.xsd`

 * *Files identical despite different names*

### Comparing `sdc11073-2.0.0a3/src/sdc11073/xsd/SafetyInformation.xsd` & `sdc11073-2.0.0a4/src/sdc11073/xsd/SafetyInformation.xsd`

 * *Files identical despite different names*

### Comparing `sdc11073-2.0.0a3/src/sdc11073/xsd/addressing.xsd` & `sdc11073-2.0.0a4/src/sdc11073/xsd/addressing.xsd`

 * *Files identical despite different names*

### Comparing `sdc11073-2.0.0a3/src/sdc11073/xsd/eventing.xsd` & `sdc11073-2.0.0a4/src/sdc11073/xsd/eventing.xsd`

 * *Files identical despite different names*

### Comparing `sdc11073-2.0.0a3/src/sdc11073/xsd/soap-envelope.xsd` & `sdc11073-2.0.0a4/src/sdc11073/xsd/soap-envelope.xsd`

 * *Files identical despite different names*

### Comparing `sdc11073-2.0.0a3/src/sdc11073/xsd/ws-addr.xsd` & `sdc11073-2.0.0a4/src/sdc11073/xsd/ws-addr.xsd`

 * *Files identical despite different names*

### Comparing `sdc11073-2.0.0a3/src/sdc11073/xsd/wsdd-discovery-1.1-schema-os.xsd` & `sdc11073-2.0.0a4/src/sdc11073/xsd/wsdd-discovery-1.1-schema-os.xsd`

 * *Files identical despite different names*

### Comparing `sdc11073-2.0.0a3/src/sdc11073/xsd/wsdd-dpws-1.1-schema-os.xsd` & `sdc11073-2.0.0a4/src/sdc11073/xsd/wsdd-dpws-1.1-schema-os.xsd`

 * *Files identical despite different names*

### Comparing `sdc11073-2.0.0a3/src/sdc11073/xsd/wsdl.xsd` & `sdc11073-2.0.0a4/src/sdc11073/xsd/wsdl.xsd`

 * *Files identical despite different names*

### Comparing `sdc11073-2.0.0a3/src/sdc11073/xsd/xml.xsd` & `sdc11073-2.0.0a4/src/sdc11073/xsd/xml.xsd`

 * *Files identical despite different names*

### Comparing `sdc11073-2.0.0a3/tutorial/README.rst` & `sdc11073-2.0.0a4/tutorial/README.rst`

 * *Files identical despite different names*

### Comparing `sdc11073-2.0.0a3/.gitignore` & `sdc11073-2.0.0a4/.gitignore`

 * *Files identical despite different names*

### Comparing `sdc11073-2.0.0a3/LICENSE` & `sdc11073-2.0.0a4/LICENSE`

 * *Files identical despite different names*

### Comparing `sdc11073-2.0.0a3/README.rst` & `sdc11073-2.0.0a4/README.rst`

 * *Files 10% similar despite different names*

```diff
@@ -70,14 +70,20 @@
     pytest
 
 Notices
 =======
 
 The sdc11073 python library is not intended for use in medical products, clinical trials, clinical studies, or in clinical routine.
 
+Limitations
+===========
+
+The wsdiscovery module only works with a single ip address. Publishing a device on multiple networks it not supported.
+The same is valid for searching.
+
 ISO 9001
 --------
 
 The sdc11073 python library was not developed according to ISO 9001.
 
 Support
 =======
```

### Comparing `sdc11073-2.0.0a3/pyproject.toml` & `sdc11073-2.0.0a4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `sdc11073-2.0.0a3/PKG-INFO` & `sdc11073-2.0.0a4/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sdc11073
-Version: 2.0.0a3
+Version: 2.0.0a4
 Summary: Pure python implementation of IEEE11073 SDC protocol
 Project-URL: Homepage, https://github.com/Draegerwerk/sdc11073
 Project-URL: Bug Tracker, https://github.com/Draegerwerk/sdc11073/issues
 Author-email: Bernd Deichmann <bernd.deichmann@draeger.com>, Leon Budnick <leon.budnick@draeger.com>
 License-File: LICENSE
 Keywords: IEEE11073,SDC
 Classifier: Development Status :: 5 - Production/Stable
@@ -101,14 +101,20 @@
     pytest
 
 Notices
 =======
 
 The sdc11073 python library is not intended for use in medical products, clinical trials, clinical studies, or in clinical routine.
 
+Limitations
+===========
+
+The wsdiscovery module only works with a single ip address. Publishing a device on multiple networks it not supported.
+The same is valid for searching.
+
 ISO 9001
 --------
 
 The sdc11073 python library was not developed according to ISO 9001.
 
 Support
 =======
```

