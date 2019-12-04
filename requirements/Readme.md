# U.S.D.O.T. Passenger Travel Requirements

1. Objectives
   1. Define the known universe of North American Transit and Intercity Bus providers (Providers).
   2. Determine if the provider publishes data according to the General Transit Feed Specification.
   3. Determine if the provider particiaptes in the Department's Passenger Travel Initiatives. (The National Transit Map (NTM) and The  Intercity Bus Atlas (ICBA))
      1. If the provider participates then, <br> harvest, compile, analyze, publish, and archive the data at least once a year but not more than 4 times a year.
      2. If the provider does not participate then <br> Flag them for contact and assign a priority based volume of service.
2. Functional Requirements
   1. Data Collection
      1. Data Tables
         1. Providers List; a list of known providers which includes their websites.
         2. Collection History; a list which tracks when a provider's website was last visited and wether or not the visit was productive. (Productive meaning GTFS data was collected.)
      2. Functions
         1. Every day, query the Visitation History table for websites which have not been visted in the last 90 days.
         2. Build a visitation schedule designed to minimize burden on provider resources.
         3. Iterate the list of sites not visited in the last 90 days, at provideres convienience, and store copies of the websites.
         4. Leave record of visitation on provider's server.				 
         5. Search website copies for GTFS URLs.
         6. Harvest raw GTFS Data
            1. Track sucessful and failed downloads in the Collection History Table
            2. Harvested raw GTFS feeds shall be stored for QC checks
         7. Email GTFS Harvest report to provider 
         8. Email GTFS Harvest Report to Dataset Manager
      3. Business Rules
         1. Be transparent when searching and harvesting from provider resources when practicable. Report to to providers when their site as been searched when possible.
         2. Collect as much metadata as possible (Work it Metadata Team to determine whats needed)
         3. Reduce burden on provider resources as much as possible. (E.g. visit site during off-peak hours)	 
   2. Data Compilation
      1. QC Checks
         1. Strip raw GTFS files of tables and fields not included in the specification
            1. Machine Read the spec
            1. Create a file which can be used to test raw GTFS files against the specification.
            1. Strip raw GTFS file of tables and fields not defined inthe specification.
         1. Assign Agency IDs to the tables and records.            
      2. Spatial Data Builds
      3. Tabular Data Builds
   3. Data Analysis
   4. Data Publication
   5. Data Archival
