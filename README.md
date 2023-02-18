# dv-flight
+-------------------+          +----------------------+        +-----------------+
|      Airline      |          |      Flight          |        |     Airport     |
+-------------------+          +----------------------+        +-----------------+
| - id: int          |          | - id: int            |        | - id: int       |
| - name: string     |          | - departureAirport:  |        | - name: string  |
+-------------------+          |    Airport           |        +-----------------+
                               | - arrivalAirport:    |
+-------------------+          |    Airport           |        +-----------------+
|       Plane       |          | - departureTime:     |        |      Pilot      |
+-------------------+          | - arrivalTime:       |        +-----------------+
| - id: int          |          | - pilot: Pilot       |        | - id: int       |
| - type: string     |          | - copilot: Pilot     |        | - name: string  |
| - airline: Airline |          | - plane: Plane       |        | - experience:   |
| - pilotsNeeded: int|          +----------------------+        |    int          |
| - isOperational:   |                                            +-----------------+
|    boolean        |
+-------------------+
                                                      
                            +------------------------+
                            |         Pilot          |
                            +------------------------+
                            | - id: int              |
                            | - name: string         |
                            | - experience: int      |
                            | - airlines: Airline[]  |
                            +------------------------+

