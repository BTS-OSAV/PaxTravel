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
         1. Maintain a Providers List; a list of known providers which includes their websites.
         2. Maintain a Visitation History; a list which tracks when a provider's website was last visited and wether or not the visit was productive. (Productive meaning GTFS data was collected.)
      2. Functions
         1. Every day, query the Visitation History table for websites which have not been visted in the last 90 days.
         2. Build a visitation schedule designed to minimize burden on provider resources.
         3. Iterate the list of sites not visited in the last 90 days, at provideres convienience, and store copies of the websites.
         4. Leave record of visitation on provider's server.				 
         5. Search website copies for useful passenger travel data.
         6. Store findings
            1. Maintain a history of actions taken
            2. Maintain a list of viable GTFS Fetch points
            3. Maintain a list of 
      3. Business Rules
         1. Collect as much metadata as possible (Work it Metadata Team to determine whats needed)
         2. Reduce burden on Provider resources as much as possible. (E.g. visit site during off-peak hours)	 
   2. Source Data Inventory
   3. Data Collection
   4. Data Storage
   5. Data Analysis	 
   6. Data Publication
   7. Data Archival
