# BP-to-BP-Tools

Tools that give the user the ability to copy "objects" from a Blueprint to 
another Blueprint. 

There are 2 groupings of tools. Group 1 provides for Blueprint to Blueprint 
copying within the same Apstra server instance. Group 2 provides for Blueprint
to Blueprint copying between 2 different Apstra server instances. Tools that 
fall into Grouping 2 will start with an "e". 

The tools require that the destination Blueprint exist. It does NOT have to
be deployed. It does NOT have to have physical devices assigned. The source and 
destination Blueprints can be based on different Templates.

```
 CTcopy - copies Connectivity Templates. It does not copy interface assignments
          since the logical devices might use a different name.  Requires that
          the RVC tool has been used to copy Route_Zones and Virtual_Networks 
          into the destination Blueprint.

eCTcopy - CTcopy for when the source Blueprint and destination Blueprint exist
          on different Apstra servers

    RVC - copies Route_Zones, Virtual_Networks, and any applied Configlets from 
          the source Blueprint to the destination Blueprint. Route_Zones and 
          Virtual_Networks to copy are selectable.

   eRVC - RVC for when the source Blueprint and destination Blueprint exist on 
          different Apstra servers with the capability to copy all Configlets
          on the source Apstra server to the destination Apstra server. Each 
          configlet is checked to be non-exist on the destination Apstra server
          before coping it. The check is based configlet name.    
```
All of the tools have a help option (-h or --help) to get more details
