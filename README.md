# Smart India Hackathon Workshop
# Date: 26/10/2026
## Register Number: 212224040375
## Name: Yugabharathi T
## Problem Title
SIH 1710: Enhancing Navigation for Railway Station Facilities and Locations
## Problem Description
Background: Railway stations are complex environments with numerous facilities and locations such as ticket counters, platforms, restrooms, food courts, and waiting areas. Passengers often face difficulties in navigating these spaces, especially in large or unfamiliar stations. Efficient and user-friendly navigation systems are crucial for improving passenger experience, reducing congestion, and ensuring timely travel connections. Description: The problem involves developing a comprehensive navigation solution for railway stations that assists passengers in locating various facilities and destinations within the station premises. This includes creating detailed maps, providing real-time directions, and integrating features such as accessibility options for individuals with disabilities. The solution should be intuitive, easy to use, and accessible via multiple platforms, including mobile devices and digital kiosks. Key challenges include updating navigation information in real-time, ensuring accuracy, and accommodating the diverse needs of all passengers. Expected Solution: The expected solution is a multi-platform navigation system that provides detailed, real-time directions to all facilities and locations within a railway station. This system should include: A mobile application with 3D interactive maps and step-by-step navigation. Digital kiosks located throughout the station with touch-screen interfaces. Voice-guided navigation for visually impaired passengers. Regular updates to reflect changes in station layout and facility locations. Integration with existing railway apps and services for seamless user experience. The solution should enhance the overall passenger experience by reducing confusion, saving time, and improving accessibility within the station.

## Problem Creater's Organization
Ministry of Railway

## Idea

SmartRail Navigator – An Accessible, Real-Time Indoor Navigation System for Railway Stations

The idea is to develop a smart navigation platform that helps passengers find platforms, ticket counters, restrooms, lifts, escalators, food courts, waiting halls, enquiry counters, and exits inside railway stations.

Unlike ordinary GPS navigation, which may not work accurately inside buildings, the proposed system uses a digital station map with indoor positioning and route guidance. Passengers can enter their destination, view the shortest or most accessible route, and follow step-by-step directions through a mobile application or a touchscreen kiosk.

The system also supports voice-guided navigation for visually impaired passengers, wheelchair-friendly routes for passengers with disabilities, and real-time updates about platform changes or temporarily unavailable facilities. This solution aims to reduce confusion, save time, improve accessibility, and help passengers reach their destinations safely.

## Proposed Solution / Architecture Diagram

The proposed system consists of a passenger interface, an indoor navigation engine, a station map database, a real-time information module, and an administrator dashboard.

<img width="946" height="737" alt="image" src="https://github.com/user-attachments/assets/abbe05f0-b80b-4cf5-8aff-ca3e18336574" />

Implementation note: A QR-code-based navigation service called Namma Nakshe already provides digital station maps at multiple stations in Bengaluru Division. Your proposed solution should distinguish itself through features such as accessibility-aware route optimization, voice-led step-by-step guidance, indoor position tracking and dynamic rerouting when pathways are blocked

## Use Cases

1. **Facility Search:** Allows passengers to find platforms, ticket counters, restrooms, food courts, waiting halls, and exits.

2. **Indoor Navigation:** Provides step-by-step directions from the passenger's current location to the selected destination.

3. **Accessible Route Planning:** Suggests wheelchair-friendly routes using ramps, accessible pathways, and available lifts.

4. **Voice-Guided Navigation:** Provides spoken directions to help visually impaired passengers navigate railway stations.

5. **Real-Time Updates:** Updates navigation information based on platform changes, facility availability, and pathway closures.

6. **Alternative Route Guidance:** Suggests alternative paths when a corridor, lift, or foot overbridge is unavailable.

7. **Digital Kiosk Assistance:** Enables passengers to search for facilities and view directions using touchscreen kiosks.

8. **Station Map Management:** Allows authorized railway staff to update station layouts, facility locations, and pathway information.



## Technology Stack

1. **Frontend Development:** Flutter for mobile application development and React.js for web applications and digital kiosks.

2. **Backend Development:** Python with FastAPI for handling navigation requests, route calculations, and station information.

3. **Database:** PostgreSQL with PostGIS for storing station maps, facility locations, and pathway information.

4. **Mapping and Visualization:** Three.js and MapLibre GL JS for interactive 2D and 3D station maps.

5. **Route Optimization:** Dijkstra's algorithm or A* algorithm for calculating the shortest and most accessible routes.

6. **Indoor Positioning:** QR codes for location identification, with optional Bluetooth Low Energy (BLE) beacons for continuous indoor positioning.

7. **Voice Navigation:** Text-to-Speech (TTS) technology for providing spoken directions to passengers.

8. **Real-Time Communication:** WebSockets for delivering updates about platform changes, facility availability, and blocked pathways.

9. **Cloud Platform:** AWS or Microsoft Azure for hosting the application, backend services, and database.

10. **Development Tools:** Visual Studio Code, Git, and GitHub for coding, version control, and team collaboration.


## Dependencies

Software dependencies

- Python 3.x and FastAPI for backend development.
- PostgreSQL with PostGIS for storing and querying station maps and locations.
- Flutter SDK for the mobile application.
- Node.js and React.js for the web application and kiosk interface.
- NetworkX or a custom graph algorithm for route calculation.
- Three.js or an equivalent mapping library for interactive 3D visualization.
- Text-to-Speech services for spoken directions.
- WebSocket support for real-time updates.
- Cloud hosting, authentication and API security components.
  
Hardware and data dependencies

- Accurate station floor plans and facility coordinates.
- Verified information about platforms, foot overbridges, subways, lifts, ramps and exits.
- Smartphones with cameras and audio output.
- Touchscreen kiosks with internet connectivity.
- Optional BLE beacons or other indoor-positioning infrastructure for more continuous location tracking.
- An administrator interface and authorized railway staff to maintain accurate station information.
- Access to official railway data or authorized integration APIs for platform and service updates.
  
Important limitations to consider

- Indoor GPS accuracy: GPS may be unreliable inside stations. QR-based starting points are practical for an initial prototype; BLE or visual positioning can be added later.
- Real-time information: Actual platform changes and lift status require an authorized data source or staff updates. The prototype should not claim live railway integration unless it is implemented.
- Map accuracy: Routes must reflect actual pathways, accessibility restrictions and temporary closures.
- Accessibility: Voice instructions should be supplemented with clear text, strong visual contrast and accessible kiosk controls.
