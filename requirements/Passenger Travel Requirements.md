# U.S.D.O.T. Passenger Travel Requirements

1. Objectives
   1. Define the known universe of North American Transit and Intercity Bus providers (Providers).
   2. Determine if the provider publishes data according to the General Transit Feed Specification.
   3. Determine if the provider particiaptes in the Department's Passenger Travel Initiatives. (The National Transit Map (NTM) and The  Intercity Bus Atlas (ICBA))
      1. If the provider participates then, <br> harvest, compile, analyze, publish, and archive the data at least once a year but not more than 4 times a year.
      2. If the provider does not participate then <br> Flag them for contact and assign a priority based volume of service.
2. Functional Requirements
   1. Data Discovery
      1. Data Tables
         1. Providers List; a list of known providers which includes their websites.
         2. Collection History; a list which tracks when a provider's website was last visited and wether or not the visit was productive. (Productive meaning GTFS data was collected.)
      2. Functions
         1. Every day, query the Visitation History table for websites which have not been visted in the last 90 days.
         2. Build a visitation schedule designed to minimize burden on provider resources.
         3. Iterate the list of sites not visited in the last 90 days, at provideres convienience, and store copies of the websites.
         4. Leave record of visitation on provider's server.				 
         5. Search website copies for GTFS URLs.
         6. Harvest GTFS Data
            1. Track Sucesses
            2. Track Failures
         7. Update Collection History
         8. Email GTFS Harvest report to provider 
         9. Email GTFS Harvest Report to Dataset Manager
      3. Business Rules
         1. When practicable, be transparent when searching and harvesting from provider resources.  Report to to providers when their site as been searched when possible.
         2. Collect as much metadata as possible (Work it Metadata Team to determine whats needed)
         3. Reduce burden on Provider resources as much as possible. (E.g. visit site during off-peak hours)	 
   2. Source Data Inventory
      1. Harvested GTFS feeds shall be stored on a USDOT server
      2. Harvested GTFS feeds shall be publically available from a URL.
   3. Data Storage
   4. Data Analysis	 
   5. Data Publication
   6. Data Archival
