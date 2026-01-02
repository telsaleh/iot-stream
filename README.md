# IoT-Stream Ontology

IoT-Stream is a lightweight extension of SOSA ontology to annotate Stream Data on the Internet of Things (IoT) context. It allows to annotate each data value in the stream or just the metadata of the stream and the location of the data.

## Background  

In recent years, the development and deployment of Internet of Things (IoT) devices has led to generation of large volumes of real world data. Analytical models can be used to extract meaningful insights from this data. However, most of IoT data is not fully utilised mainly due to interoperability issues and the difficulties to analyse data collected by heterogeneous resources. To overcome this heterogeneity, semantic technologies are sued to create common models to share various data originated from heterogeneous sources. However, semantics add further overhead to the data communication and the processing time to annotate the data with the model can increase the latency and complexity in publishing and querying the annotated data. We present a lightweight semantic model to annotate IoT streams. The metadata descriptions that are provided in the models are used for search and discovery of the data using various attributes such as value and type. The proposed model extends the commonly used ontologies such as W3C/OGC SSN ontology and its recent lightweight core, SOSA, and includes concepts to describe streaming IoT data.

The rapid growth of Internet of Things (IoT) devices has increased the amount of data that is collected and communicated from real world environments. The IoT data is often collected by various devices and is represented in different forms. The heterogeneity of the data and interoperability issues between different sources and platforms is a common challenge in creating large-scale IoT data analytics services and applications.

## What it is
A lightweight semantic model for the annotation of stream data, IoT-Stream, that extends SOSA, (and by extension SSN) ontology, and therefore is fully compatible with SOSA. In our proposal we have centred the attention around the stream data. To keep it simple, each stream observation contains only a value and a timestamp. To that end, we have taken outside the stream observation, all the needed metadata useful for searching purposes, but unnecessary for the (quasi) real-time processing of the data. In our model, not only raw data can be annotated as streams, but also processed data. The processed data is also kept lightweight. For example, raw data coming from a sensor that it is produced every minute can be individually annotated. However, if such fine granularity is not needed, data can be aggregated in windows of 5 minutes using data mining algorithms, such as SAX (Symbolic Aggregate Approximation), and annotate the processed stream data. These aggregated stream annotations are still lightweight, with only the annotations of the aggregated value and the start/end times of the aggregated value. Metadata for searching purposes is also appended, such as algorithm used, values of the parameters of the algorithm, etc., outside of the stream observations.

## Publications:

- Elsaleh, T.; Enshaeifar, S.; Rezvani, R.; Acton, S.T.; Janeiko, V.; Bermudez-Edo, M. IoT-Stream: A Lightweight Ontology for Internet of Things Data Streams and Its Use with Data Analytics and Event Detection Services. Sensors 2020, 20, 953. https://doi.org/10.3390/s20040953.
- T. Elsaleh, M. Bermudez-Edo, S. Enshaeifar, S. T. Acton, R. Rezvani and P. Barnaghi, "IoT-Stream: A Lightweight Ontology for Internet of Things Data Streams," 2019 Global IoT Summit (GIoTS), Aarhus, Denmark, 2019, pp. 1-6, doi: 10.1109/GIOTS.2019.8766367.

## Namespaces
- ```iot-stream```: ``` http://purl.org/iot/ontology/iot-stream ```
- ```schema```:	```<http://schema.org>```
- ``iot-lite```:	```<http://purl.oclc.org/NET/UNIS/fiware/iot-lite>```
- ```qu```:	```<http://purl.oclc.org/NET/ssnx/qu/qu>```
- ```sosa```:	```<http://www.w3.org/ns/sosa>```
- ```ns```:	```<http://www.w3.org/2003/06/sw-vocab-status/ns>```
- ```owl```:	```<http://www.w3.org/2002/07/owl>```
- ```xsd```:	```<http://www.w3.org/2001/XMLSchema>```
- ```skos```:	```<http://www.w3.org/2004/02/skos/core>```
- ```qoi```:	```<https://w3id.org/iot/qoi>```
- ```rdfs```:	```<http://www.w3.org/2000/01/rdf-schema>```
- ```geosparql```:	```<http://www.opengis.net/ont/geosparql>```
- ```rdf```:	```<http://www.w3.org/1999/02/22-rdf-syntax-ns>```
- ```terms```:	```<http://purl.org/dc/terms>```
- ```bibo```:	```<http://purl.org/ontology/bibo>```
- ```wgs84_pos```:	```<http://www.w3.org/2003/01/geo/wgs84_pos>```
- ```vann```:	```<http://purl.org/vocab/vann>```
- ```dc```:	```<http://purl.org/dc/elements/1.1>```

## Funding
This work has been funded by the EU Horizon 2020 Research and Innovation programme, through projects IoTCrawler (contract no. 779852) and ACTIVAGE (contract no. 732679).
