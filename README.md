**Sensor for Plugwise Smile P1 integration**

Initial source code from https://bitbucket.org/jvdschoot/home-assistant-sensor-plugwise-smile-p1/src/master/

Usage:

You most probably need to install the additional package `lxml` via the command `pip3 install lxml`.
       
      sensor:
      - platform: plugwisesmile
        name: Plugwise Smile
        host: x.x.x.x
        username: smile
        password: password
        resources:
          - electricity_consumed_point
          - electricity_consumed_offpeak_interval
          - electricity_consumed_peak_interval
          - electricity_consumed_offpeak_cumulative
          - electricity_consumed_peak_cumulative
          - electricity_produced_point
          - electricity_produced_offpeak_interval
          - electricity_produced_peak_interval
          - electricity_produced_offpeak_cumulative
          - electricity_produced_peak_cumulative
          - gas_consumed_interval
          - gas_consumed_cumulative
