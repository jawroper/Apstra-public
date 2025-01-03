# Apstra-public

Scripts that allow the user to retrieve (ie dump) and/or insert specific custom
settings from and/or to an Apstra server.

getDPSCCW - is an "uber" retrieval script. It allows the user to retrieve
            Dashboards, Probes, Services, Collectors, Configlets, or Widgets

postDPSCCW - is an "uber" insert script. It allows the user to insert Dashboards,
             Probes, Services, Collectors, Configlets, or Widgets

Tools that start with "dump" perform a very specific retrieval.

Retrieved settings can be output to the terminal or to an output file.  When
sent to an output file(s) the filename will end with one of the following:

      _dash.json for each retrieved Dashboard
      _prob.json for each retrieved Probe
      _serv.json for each retrieved Service Registry
      _coll.json for each retrieved Collector
      _cflt.json for each retrieved Configlet
      _widg.json for each retrieved Widget

      Note:  Since Dashboards, Probes, and Widgets are Blueprint specific,
             the output filename will also contain the Blueprint name.


UUIDchg - for a complete explanation read its built in help "UUIDchg -h"
