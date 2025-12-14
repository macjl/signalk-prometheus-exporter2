# Signal K to Prometheus Plugin

Forked from https://github.com/ieb/signalk-prometheus-exporter

Signal K Node server plugin to make a Prometheus pull end point to allow a Prometheus server to pull data.

To use, install a Prometheus server and configure it to pull from 

http://localhost:3000/signalk/v1/api/prometheus

which will contain the current values eg

    # HELP navigation_speedOverGround navigation_speedOverGround
    # TYPE navigation_speedOverGround gauge
    navigation_speedOverGround{context="vessels.urn:mrn:imo:mmsi:227400000",source="Can0.1"} 3.155 1765750269678
    # HELP environment_mode environment_mode
    # TYPE environment_mode gauge
    environment_mode{context="vessels.urn:mrn:imo:mmsi:227400000",source="derived-data",value_str="night"} 1 1765750245374
    # HELP navigation_position_longitude navigation_position_longitude
    # TYPE navigation_position_longitude gauge
    navigation_position_longitude{context="vessels.urn:mrn:imo:mmsi:227400000",source="Can0.1"} 17.1383474 1765750269680
    # HELP navigation_position_latitude navigation_position_latitude
    # TYPE navigation_position_latitude gauge
    navigation_position_latitude{context="vessels.urn:mrn:imo:mmsi:227400000",source="Can0.1"} 23.6357923 176575026968
