# Comparing `tmp/omie-0.0.0.tar.gz` & `tmp/omie-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/omie-0.0.0.tar", last modified: Mon Mar  4 15:27:15 2024, max compression
+gzip compressed data, was "omie-0.1.0.tar", last modified: Tue May  7 12:44:29 2024, max compression
```

## Comparing `omie-0.0.0.tar` & `omie-0.1.0.tar`

### file list

```diff
@@ -1,15 +1,121 @@
-drwxrwxr-x   0 aorellana  (1000) aorellana  (1000)        0 2024-03-04 15:27:15.000000 omie-0.0.0/
--rw-rw-r--   0 aorellana  (1000) aorellana  (1000)      278 2024-03-04 15:27:15.000000 omie-0.0.0/PKG-INFO
-drwxrwxr-x   0 aorellana  (1000) aorellana  (1000)        0 2024-03-04 15:27:15.000000 omie-0.0.0/omie/
--rw-rw-r--   0 aorellana  (1000) aorellana  (1000)       96 2024-03-04 14:30:09.000000 omie-0.0.0/omie/omie.py
--rw-rw-r--   0 aorellana  (1000) aorellana  (1000)       46 2024-03-04 14:42:05.000000 omie-0.0.0/omie/__init__.py
--rw-rw-r--   0 aorellana  (1000) aorellana  (1000)      230 2024-03-04 14:21:06.000000 omie-0.0.0/README.md
--rw-rw-r--   0 aorellana  (1000) aorellana  (1000)       38 2024-03-04 15:27:15.000000 omie-0.0.0/setup.cfg
--rw-rw-r--   0 aorellana  (1000) aorellana  (1000)     1244 2024-03-04 14:54:12.000000 omie-0.0.0/setup.py
-drwxrwxr-x   0 aorellana  (1000) aorellana  (1000)        0 2024-03-04 15:27:15.000000 omie-0.0.0/omie.egg-info/
--rw-rw-r--   0 aorellana  (1000) aorellana  (1000)        1 2024-03-04 15:27:15.000000 omie-0.0.0/omie.egg-info/dependency_links.txt
--rw-rw-r--   0 aorellana  (1000) aorellana  (1000)      278 2024-03-04 15:27:15.000000 omie-0.0.0/omie.egg-info/PKG-INFO
--rw-rw-r--   0 aorellana  (1000) aorellana  (1000)        5 2024-03-04 15:27:15.000000 omie-0.0.0/omie.egg-info/requires.txt
--rw-rw-r--   0 aorellana  (1000) aorellana  (1000)        5 2024-03-04 15:27:15.000000 omie-0.0.0/omie.egg-info/top_level.txt
--rw-rw-r--   0 aorellana  (1000) aorellana  (1000)       52 2024-03-04 15:27:15.000000 omie-0.0.0/omie.egg-info/entry_points.txt
--rw-rw-r--   0 aorellana  (1000) aorellana  (1000)      218 2024-03-04 15:27:15.000000 omie-0.0.0/omie.egg-info/SOURCES.txt
+drwxrwxr-x   0 aorellana  (1000) aorellana  (1000)        0 2024-05-07 12:44:29.626413 omie-0.1.0/
+-rw-r--r--   0 aorellana  (1000) aorellana  (1000)      268 2024-05-07 12:44:29.626413 omie-0.1.0/PKG-INFO
+-rw-rw-r--   0 aorellana  (1000) aorellana  (1000)      230 2024-05-07 12:42:42.000000 omie-0.1.0/README.md
+drwxrwxr-x   0 aorellana  (1000) aorellana  (1000)        0 2024-05-07 12:44:29.606413 omie-0.1.0/omie/
+-rw-rw-r--   0 aorellana  (1000) aorellana  (1000)       55 2024-05-07 12:42:42.000000 omie-0.1.0/omie/__init__.py
+-rw-rw-r--   0 aorellana  (1000) aorellana  (1000)     5904 2024-05-07 12:42:57.000000 omie-0.1.0/omie/omie.py
+drwxrwxr-x   0 aorellana  (1000) aorellana  (1000)        0 2024-05-07 12:44:29.610413 omie-0.1.0/omie/services/
+-rw-rw-r--   0 aorellana  (1000) aorellana  (1000)     2096 2024-05-07 12:42:42.000000 omie-0.1.0/omie/services/ServicioAltaDesagregacionesCP.wsdl
+-rw-rw-r--   0 aorellana  (1000) aorellana  (1000)     2096 2024-05-07 12:42:42.000000 omie-0.1.0/omie/services/ServicioAltaDesagregacionesMC.wsdl
+-rw-rw-r--   0 aorellana  (1000) aorellana  (1000)     2156 2024-05-07 12:42:42.000000 omie-0.1.0/omie/services/ServicioAltaEnergiasComprometidas.wsdl
+-rw-rw-r--   0 aorellana  (1000) aorellana  (1000)     2183 2024-05-07 12:42:42.000000 omie-0.1.0/omie/services/ServicioAltaMessagesUmmElectricity.wsdl
+-rw-rw-r--   0 aorellana  (1000) aorellana  (1000)     2117 2024-05-07 12:42:42.000000 omie-0.1.0/omie/services/ServicioAltaMessagesUmmOther.wsdl
+-rw-rw-r--   0 aorellana  (1000) aorellana  (1000)     1970 2024-05-07 12:42:42.000000 omie-0.1.0/omie/services/ServicioAltaOfertasMD.wsdl
+-rw-rw-r--   0 aorellana  (1000) aorellana  (1000)     1969 2024-05-07 12:42:42.000000 omie-0.1.0/omie/services/ServicioAltaOfertasMI.wsdl
+-rw-rw-r--   0 aorellana  (1000) aorellana  (1000)     2093 2024-05-07 12:42:42.000000 omie-0.1.0/omie/services/ServicioAnulacionOfertasMD.wsdl
+-rw-rw-r--   0 aorellana  (1000) aorellana  (1000)     2150 2024-05-07 12:42:42.000000 omie-0.1.0/omie/services/ServicioAnulacionOfertasMIAgente.wsdl
+-rw-rw-r--   0 aorellana  (1000) aorellana  (1000)     2147 2024-05-07 12:42:42.000000 omie-0.1.0/omie/services/ServicioAnulacionOfertasMIUnidad.wsdl
+-rw-rw-r--   0 aorellana  (1000) aorellana  (1000)     1902 2024-05-07 12:42:42.000000 omie-0.1.0/omie/services/ServicioConsultaDatosUsuario.wsdl
+-rw-rw-r--   0 aorellana  (1000) aorellana  (1000)     2138 2024-05-07 12:42:42.000000 omie-0.1.0/omie/services/ServicioConsultaDesagregacionesCP.wsdl
+-rw-rw-r--   0 aorellana  (1000) aorellana  (1000)     2138 2024-05-07 12:42:42.000000 omie-0.1.0/omie/services/ServicioConsultaDesagregacionesMC.wsdl
+-rw-rw-r--   0 aorellana  (1000) aorellana  (1000)     1837 2024-05-07 12:42:42.000000 omie-0.1.0/omie/services/ServicioConsultaFechaHora.wsdl
+-rw-rw-r--   0 aorellana  (1000) aorellana  (1000)     2708 2024-05-07 12:42:42.000000 omie-0.1.0/omie/services/ServicioConsultaMercados.wsdl
+-rw-rw-r--   0 aorellana  (1000) aorellana  (1000)     2042 2024-05-07 12:42:42.000000 omie-0.1.0/omie/services/ServicioConsultaOfertasMD.wsdl
+-rw-rw-r--   0 aorellana  (1000) aorellana  (1000)     2042 2024-05-07 12:42:42.000000 omie-0.1.0/omie/services/ServicioConsultaOfertasMI.wsdl
+-rw-rw-r--   0 aorellana  (1000) aorellana  (1000)     2036 2024-05-07 12:42:42.000000 omie-0.1.0/omie/services/ServicioConsultaUmm.wsdl
+-rw-rw-r--   0 aorellana  (1000) aorellana  (1000)     2015 2024-05-07 12:42:42.000000 omie-0.1.0/omie/services/ServicioDescargaREMIT.wsdl
+-rw-rw-r--   0 aorellana  (1000) aorellana  (1000)     4126 2024-05-07 12:42:42.000000 omie-0.1.0/omie/services/ServiciosConsultaDocumento.wsdl
+-rw-rw-r--   0 aorellana  (1000) aorellana  (1000)     5754 2024-05-07 12:42:42.000000 omie-0.1.0/omie/services/ServiciosConsultas.wsdl
+-rw-rw-r--   0 aorellana  (1000) aorellana  (1000)     5324 2024-05-07 12:42:42.000000 omie-0.1.0/omie/services/ServiciosConsultasAuxiliares.wsdl
+-rw-rw-r--   0 aorellana  (1000) aorellana  (1000)     2748 2024-05-07 12:42:42.000000 omie-0.1.0/omie/services/ServiciosIdiomas.wsdl
+drwxrwxr-x   0 aorellana  (1000) aorellana  (1000)        0 2024-05-07 12:44:29.626413 omie-0.1.0/omie/xsd/
+-rw-rw-r--   0 aorellana  (1000) aorellana  (1000)   183600 2024-05-07 12:42:42.000000 omie-0.1.0/omie/xsd/Facturaev3_2_1.xsd
+-rw-rw-r--   0 aorellana  (1000) aorellana  (1000)    10953 2024-05-07 12:42:42.000000 omie-0.1.0/omie/xsd/InfoMercado.xsd
+-rw-rw-r--   0 aorellana  (1000) aorellana  (1000)    16966 2024-05-07 12:42:42.000000 omie-0.1.0/omie/xsd/MensajeAnotaciones.xsd
+-rw-rw-r--   0 aorellana  (1000) aorellana  (1000)     3916 2024-05-07 12:42:42.000000 omie-0.1.0/omie/xsd/MensajeAnulacionDeclaracionesREFechaMD.xsd
+-rw-rw-r--   0 aorellana  (1000) aorellana  (1000)     4331 2024-05-07 12:42:42.000000 omie-0.1.0/omie/xsd/MensajeAnulacionDeclaracionesREFechaMI.xsd
+-rw-rw-r--   0 aorellana  (1000) aorellana  (1000)     3940 2024-05-07 12:42:42.000000 omie-0.1.0/omie/xsd/MensajeAnulacionDesagregacionesCP.xsd
+-rw-rw-r--   0 aorellana  (1000) aorellana  (1000)     3827 2024-05-07 12:42:42.000000 omie-0.1.0/omie/xsd/MensajeAnulacionEjecucionesCBFFecha.xsd
+-rw-rw-r--   0 aorellana  (1000) aorellana  (1000)     3556 2024-05-07 12:42:42.000000 omie-0.1.0/omie/xsd/MensajeAnulacionEnergiaComprometida.xsd
+-rw-rw-r--   0 aorellana  (1000) aorellana  (1000)     3942 2024-05-07 12:42:42.000000 omie-0.1.0/omie/xsd/MensajeAnulacionExcedentesREDFecha.xsd
+-rw-rw-r--   0 aorellana  (1000) aorellana  (1000)     4396 2024-05-07 12:42:42.000000 omie-0.1.0/omie/xsd/MensajeAnulacionOfertaSesionMI.xsd
+-rw-rw-r--   0 aorellana  (1000) aorellana  (1000)     4144 2024-05-07 12:42:42.000000 omie-0.1.0/omie/xsd/MensajeAnulacionOfertasAgenteMI.xsd
+-rw-rw-r--   0 aorellana  (1000) aorellana  (1000)     3772 2024-05-07 12:42:42.000000 omie-0.1.0/omie/xsd/MensajeAnulacionOfertasFechaMD.xsd
+-rw-rw-r--   0 aorellana  (1000) aorellana  (1000)     8198 2024-05-07 12:42:42.000000 omie-0.1.0/omie/xsd/MensajeCBF.xsd
+-rw-rw-r--   0 aorellana  (1000) aorellana  (1000)     1645 2024-05-07 12:42:42.000000 omie-0.1.0/omie/xsd/MensajeCSV.xsd
+-rw-rw-r--   0 aorellana  (1000) aorellana  (1000)     7355 2024-05-07 12:42:42.000000 omie-0.1.0/omie/xsd/MensajeCapacidadIntercambio.xsd
+-rw-rw-r--   0 aorellana  (1000) aorellana  (1000)     9665 2024-05-07 12:42:42.000000 omie-0.1.0/omie/xsd/MensajeCertificadosExportacion.xsd
+-rw-rw-r--   0 aorellana  (1000) aorellana  (1000)     1436 2024-05-07 12:42:42.000000 omie-0.1.0/omie/xsd/MensajeConsultaDatosEnviados.xsd
+-rw-rw-r--   0 aorellana  (1000) aorellana  (1000)     2084 2024-05-07 12:42:42.000000 omie-0.1.0/omie/xsd/MensajeConsultaFactura.xsd
+-rw-rw-r--   0 aorellana  (1000) aorellana  (1000)     1746 2024-05-07 12:42:42.000000 omie-0.1.0/omie/xsd/MensajeConsultaUMM.xsd
+-rw-rw-r--   0 aorellana  (1000) aorellana  (1000)     2370 2024-05-07 12:42:42.000000 omie-0.1.0/omie/xsd/MensajeDatosAgente.xsd
+-rw-rw-r--   0 aorellana  (1000) aorellana  (1000)     5829 2024-05-07 12:42:42.000000 omie-0.1.0/omie/xsd/MensajeDeclExcedREDMD.xsd
+-rw-rw-r--   0 aorellana  (1000) aorellana  (1000)     5966 2024-05-07 12:42:42.000000 omie-0.1.0/omie/xsd/MensajeDeclExcedREDMI.xsd
+-rw-rw-r--   0 aorellana  (1000) aorellana  (1000)     7180 2024-05-07 12:42:42.000000 omie-0.1.0/omie/xsd/MensajeDesagregaciones.xsd
+-rw-rw-r--   0 aorellana  (1000) aorellana  (1000)     6386 2024-05-07 12:42:43.000000 omie-0.1.0/omie/xsd/MensajeDesagregacionesCP.xsd
+-rw-rw-r--   0 aorellana  (1000) aorellana  (1000)     6164 2024-05-07 12:42:43.000000 omie-0.1.0/omie/xsd/MensajeDesagregacionesMC.xsd
+-rw-rw-r--   0 aorellana  (1000) aorellana  (1000)     6451 2024-05-07 12:42:43.000000 omie-0.1.0/omie/xsd/MensajeDesgloses.xsd
+-rw-rw-r--   0 aorellana  (1000) aorellana  (1000)     7546 2024-05-07 12:42:43.000000 omie-0.1.0/omie/xsd/MensajeEjecCBF.xsd
+-rw-rw-r--   0 aorellana  (1000) aorellana  (1000)     5116 2024-05-07 12:42:43.000000 omie-0.1.0/omie/xsd/MensajeEjecucionConsulta.xsd
+-rw-rw-r--   0 aorellana  (1000) aorellana  (1000)     5668 2024-05-07 12:42:43.000000 omie-0.1.0/omie/xsd/MensajeEnergiasComprometidas.xsd
+-rw-rw-r--   0 aorellana  (1000) aorellana  (1000)     6043 2024-05-07 12:42:43.000000 omie-0.1.0/omie/xsd/MensajeEnergiasTotales.xsd
+-rw-rw-r--   0 aorellana  (1000) aorellana  (1000)     5741 2024-05-07 12:42:43.000000 omie-0.1.0/omie/xsd/MensajeExcedRED.xsd
+-rw-rw-r--   0 aorellana  (1000) aorellana  (1000)     2212 2024-05-07 12:42:43.000000 omie-0.1.0/omie/xsd/MensajeFicherosNuevos.xsd
+-rw-rw-r--   0 aorellana  (1000) aorellana  (1000)     3345 2024-05-07 12:42:43.000000 omie-0.1.0/omie/xsd/MensajeFicherosNuevosFact.xsd
+-rw-rw-r--   0 aorellana  (1000) aorellana  (1000)     2860 2024-05-07 12:42:43.000000 omie-0.1.0/omie/xsd/MensajeFicherosNuevosLiq.xsd
+-rw-rw-r--   0 aorellana  (1000) aorellana  (1000)     5228 2024-05-07 12:42:43.000000 omie-0.1.0/omie/xsd/MensajeHorasAnuladas.xsd
+-rw-rw-r--   0 aorellana  (1000) aorellana  (1000)     5221 2024-05-07 12:42:43.000000 omie-0.1.0/omie/xsd/MensajeHorasAnuladasContinuo.xsd
+-rw-rw-r--   0 aorellana  (1000) aorellana  (1000)     5185 2024-05-07 12:42:43.000000 omie-0.1.0/omie/xsd/MensajeImportesAcumulados.xsd
+-rw-rw-r--   0 aorellana  (1000) aorellana  (1000)     9800 2024-05-07 12:42:43.000000 omie-0.1.0/omie/xsd/MensajeOfertasMD.xsd
+-rw-rw-r--   0 aorellana  (1000) aorellana  (1000)    18381 2024-05-07 12:42:43.000000 omie-0.1.0/omie/xsd/MensajeOfertasMI.xsd
+-rw-rw-r--   0 aorellana  (1000) aorellana  (1000)     4121 2024-05-07 12:42:43.000000 omie-0.1.0/omie/xsd/MensajeOfertasSubastasInterconexion.xsd
+-rw-rw-r--   0 aorellana  (1000) aorellana  (1000)     5945 2024-05-07 12:42:43.000000 omie-0.1.0/omie/xsd/MensajePrecios.xsd
+-rw-rw-r--   0 aorellana  (1000) aorellana  (1000)     5358 2024-05-07 12:42:43.000000 omie-0.1.0/omie/xsd/MensajePreciosContinuo.xsd
+-rw-rw-r--   0 aorellana  (1000) aorellana  (1000)     3560 2024-05-07 12:42:43.000000 omie-0.1.0/omie/xsd/MensajePreciosGasNatural.xsd
+-rw-rw-r--   0 aorellana  (1000) aorellana  (1000)     7257 2024-05-07 12:42:43.000000 omie-0.1.0/omie/xsd/MensajePrograma.xsd
+-rw-rw-r--   0 aorellana  (1000) aorellana  (1000)     6209 2024-05-07 12:42:43.000000 omie-0.1.0/omie/xsd/MensajeProgramaContinuo.xsd
+-rw-rw-r--   0 aorellana  (1000) aorellana  (1000)     2945 2024-05-07 12:42:43.000000 omie-0.1.0/omie/xsd/MensajeRetiradaDeclaracionesDefectoRE.xsd
+-rw-rw-r--   0 aorellana  (1000) aorellana  (1000)     2920 2024-05-07 12:42:43.000000 omie-0.1.0/omie/xsd/MensajeRetiradaEjecucionesCBFDefecto.xsd
+-rw-rw-r--   0 aorellana  (1000) aorellana  (1000)     2861 2024-05-07 12:42:43.000000 omie-0.1.0/omie/xsd/MensajeRetiradaOfertasDefectoMD.xsd
+-rw-rw-r--   0 aorellana  (1000) aorellana  (1000)     1892 2024-05-07 12:42:43.000000 omie-0.1.0/omie/xsd/MensajeServicioDescargaREMIT.xsd
+-rw-rw-r--   0 aorellana  (1000) aorellana  (1000)     7453 2024-05-07 12:42:43.000000 omie-0.1.0/omie/xsd/MensajeTransaccionesContinuo.xsd
+-rw-rw-r--   0 aorellana  (1000) aorellana  (1000)     5730 2024-05-07 12:42:43.000000 omie-0.1.0/omie/xsd/REMITUMMCommonSchema_V1.xsd
+-rw-rw-r--   0 aorellana  (1000) aorellana  (1000)    11314 2024-05-07 12:42:43.000000 omie-0.1.0/omie/xsd/REMITUMMElectricitySchema_V2.xsd
+-rw-rw-r--   0 aorellana  (1000) aorellana  (1000)     4894 2024-05-07 12:42:43.000000 omie-0.1.0/omie/xsd/REMITUMMOtherSchema_V1.xsd
+-rw-rw-r--   0 aorellana  (1000) aorellana  (1000)     4771 2024-05-07 12:42:43.000000 omie-0.1.0/omie/xsd/RespuestaAnulacionDesagregacionesCP.xsd
+-rw-rw-r--   0 aorellana  (1000) aorellana  (1000)     4950 2024-05-07 12:42:43.000000 omie-0.1.0/omie/xsd/RespuestaAnulacionRetiradaEjecucionesCBF.xsd
+-rw-rw-r--   0 aorellana  (1000) aorellana  (1000)     4909 2024-05-07 12:42:43.000000 omie-0.1.0/omie/xsd/RespuestaAnulacionRetiradaOfertas.xsd
+-rw-rw-r--   0 aorellana  (1000) aorellana  (1000)     5055 2024-05-07 12:42:43.000000 omie-0.1.0/omie/xsd/RespuestaAnulacionRetiradaRE.xsd
+-rw-rw-r--   0 aorellana  (1000) aorellana  (1000)    16083 2024-05-07 12:42:43.000000 omie-0.1.0/omie/xsd/RespuestaConfiguracionConsulta.xsd
+-rw-rw-r--   0 aorellana  (1000) aorellana  (1000)    11060 2024-05-07 12:42:43.000000 omie-0.1.0/omie/xsd/RespuestaDatosUsuario.xsd
+-rw-rw-r--   0 aorellana  (1000) aorellana  (1000)     6106 2024-05-07 12:42:43.000000 omie-0.1.0/omie/xsd/RespuestaDeclExcedRED.xsd
+-rw-rw-r--   0 aorellana  (1000) aorellana  (1000)     6152 2024-05-07 12:42:43.000000 omie-0.1.0/omie/xsd/RespuestaDesagregaciones.xsd
+-rw-rw-r--   0 aorellana  (1000) aorellana  (1000)     6023 2024-05-07 12:42:43.000000 omie-0.1.0/omie/xsd/RespuestaDesagregacionesCP.xsd
+-rw-rw-r--   0 aorellana  (1000) aorellana  (1000)     6262 2024-05-07 12:42:43.000000 omie-0.1.0/omie/xsd/RespuestaDesagregacionesMC.xsd
+-rw-rw-r--   0 aorellana  (1000) aorellana  (1000)     1869 2024-05-07 12:42:43.000000 omie-0.1.0/omie/xsd/RespuestaDescargaREMIT.xsd
+-rw-rw-r--   0 aorellana  (1000) aorellana  (1000)     6090 2024-05-07 12:42:43.000000 omie-0.1.0/omie/xsd/RespuestaDesgloses.xsd
+-rw-rw-r--   0 aorellana  (1000) aorellana  (1000)     3190 2024-05-07 12:42:43.000000 omie-0.1.0/omie/xsd/RespuestaDirectorioConsultas.xsd
+-rw-rw-r--   0 aorellana  (1000) aorellana  (1000)     5989 2024-05-07 12:42:43.000000 omie-0.1.0/omie/xsd/RespuestaEjecCBF.xsd
+-rw-rw-r--   0 aorellana  (1000) aorellana  (1000)     7196 2024-05-07 12:42:43.000000 omie-0.1.0/omie/xsd/RespuestaEjecucionConsultaAnexo.xsd
+-rw-rw-r--   0 aorellana  (1000) aorellana  (1000)    14630 2024-05-07 12:42:43.000000 omie-0.1.0/omie/xsd/RespuestaEjecucionConsultaEncolumnada.xsd
+-rw-rw-r--   0 aorellana  (1000) aorellana  (1000)     1586 2024-05-07 12:42:43.000000 omie-0.1.0/omie/xsd/RespuestaEjecucionConsultaPrograma.xsd
+-rw-rw-r--   0 aorellana  (1000) aorellana  (1000)     5641 2024-05-07 12:42:43.000000 omie-0.1.0/omie/xsd/RespuestaEnergiasComprometidas.xsd
+-rw-rw-r--   0 aorellana  (1000) aorellana  (1000)     6015 2024-05-07 12:42:43.000000 omie-0.1.0/omie/xsd/RespuestaExcedRED.xsd
+-rw-rw-r--   0 aorellana  (1000) aorellana  (1000)     4770 2024-05-07 12:42:43.000000 omie-0.1.0/omie/xsd/RespuestaFicherosNuevos.xsd
+-rw-rw-r--   0 aorellana  (1000) aorellana  (1000)     4926 2024-05-07 12:42:43.000000 omie-0.1.0/omie/xsd/RespuestaFicherosNuevosFact.xsd
+-rw-rw-r--   0 aorellana  (1000) aorellana  (1000)     5317 2024-05-07 12:42:43.000000 omie-0.1.0/omie/xsd/RespuestaFicherosNuevosLiq.xsd
+-rw-rw-r--   0 aorellana  (1000) aorellana  (1000)     2532 2024-05-07 12:42:43.000000 omie-0.1.0/omie/xsd/RespuestaListadoIdiomas.xsd
+-rw-rw-r--   0 aorellana  (1000) aorellana  (1000)     2170 2024-05-07 12:42:43.000000 omie-0.1.0/omie/xsd/RespuestaMensajesCortosActivos.xsd
+-rw-rw-r--   0 aorellana  (1000) aorellana  (1000)     5915 2024-05-07 12:42:43.000000 omie-0.1.0/omie/xsd/RespuestaOfertas.xsd
+-rw-rw-r--   0 aorellana  (1000) aorellana  (1000)    10557 2024-05-07 12:42:43.000000 omie-0.1.0/omie/xsd/RespuestaTiposFicheros.xsd
+-rw-rw-r--   0 aorellana  (1000) aorellana  (1000)    77065 2024-05-07 12:42:43.000000 omie-0.1.0/omie/xsd/eFactura_AEAT-CCI.xsd
+-rw-rw-r--   0 aorellana  (1000) aorellana  (1000)    48321 2024-05-07 12:42:43.000000 omie-0.1.0/omie/xsd/tiposOMEL.xsd
+drwxrwxr-x   0 aorellana  (1000) aorellana  (1000)        0 2024-05-07 12:44:29.606413 omie-0.1.0/omie.egg-info/
+-rw-r--r--   0 aorellana  (1000) aorellana  (1000)      268 2024-05-07 12:44:29.000000 omie-0.1.0/omie.egg-info/PKG-INFO
+-rw-rw-r--   0 aorellana  (1000) aorellana  (1000)     4410 2024-05-07 12:44:29.000000 omie-0.1.0/omie.egg-info/SOURCES.txt
+-rw-rw-r--   0 aorellana  (1000) aorellana  (1000)        1 2024-05-07 12:44:29.000000 omie-0.1.0/omie.egg-info/dependency_links.txt
+-rw-rw-r--   0 aorellana  (1000) aorellana  (1000)       37 2024-05-07 12:44:29.000000 omie-0.1.0/omie.egg-info/entry_points.txt
+-rw-rw-r--   0 aorellana  (1000) aorellana  (1000)        5 2024-05-07 12:44:29.000000 omie-0.1.0/omie.egg-info/requires.txt
+-rw-rw-r--   0 aorellana  (1000) aorellana  (1000)        5 2024-05-07 12:44:29.000000 omie-0.1.0/omie.egg-info/top_level.txt
+-rw-rw-r--   0 aorellana  (1000) aorellana  (1000)       38 2024-05-07 12:44:29.626413 omie-0.1.0/setup.cfg
+-rw-rw-r--   0 aorellana  (1000) aorellana  (1000)     1284 2024-05-07 12:42:57.000000 omie-0.1.0/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `omie-0.0.0/setup.py` & `omie-0.1.0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from __future__ import print_function
 
 import os
 import shutil
 from distutils.command.clean import clean as _clean
 from setuptools import setup, find_packages
 
-PACKAGES_DATA = {'omie': ['data/*.xsd']}
+PACKAGES_DATA = {'omie': ['services/*.wsdl', 'xsd/*.xsd']}
 
 with open('requirements.txt', 'r') as f:
     INSTALL_REQUIRES = f.readlines()
 
 
 class Clean(_clean):
     """Eliminem el directory build i els bindings creats."""
@@ -22,14 +22,15 @@
         if os.path.exists(self.build_base):
             print("Cleaning {} dir".format(self.build_base))
             shutil.rmtree(self.build_base)
 
 
 setup(
     name='omie',
+    version='0.1.0',
     description='Libreria de interacción con OMIE',
     author='Adrià Orellana',
     author_email='aorellana@gisce.net',
     url='http://www.gisce.net',
     license='General Public Licence 2',
     long_description='''Long description''',
     provides=['omie'],
```

