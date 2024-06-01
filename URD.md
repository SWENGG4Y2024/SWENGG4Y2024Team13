# User Requirements Document

## Table of Contents

1. [Onboarding:](#onboarding)
   - [User Information and Preferences](#user-information-and-preferences)
   - [Crop Selection and Size Input](#crop-selection-and-size-input)

2. [Guide The User Page (Homepage):](#guide-the-user-page-homepage)
   - [Today's Todos and Weather](#todays-todos-and-weather)
   - [Latest Developments](#latest-developments)
   - [Current Market Price](#current-market-price)
   - [Reminder for Journal Entry](#reminder-for-journal-entry)

3. [Features on Separate Pages:](#features-on-separate-pages)
   1. [Chat Room](#1-chat-room)
   2. [Calendar](#2-calendar)
   3. [Journal](#3-journal)
   4. [Insights and Recommendations](#4-insights-and-recommendations)
   5. [Autopilot Farming](#5-autopilot-farming)
      
4. [Software Reviews:](#software-reviews)
5. [Simulation and Prototyping:](#simulation-and-prototyping)
6. [Measures for Software Assessment:](#measures-for-software-assessment)
   - [Function-based (Structured) Design Measures:](#function-based-structured-design-measures)
     1. [Analyzing Functional Decomposition:](#analyzing-functional-decomposition)
     2. [Measuring Module Size, Complexity Metrics, Coupling, Cohesion, and Hierarchical Depth:](#measuring-module-size-complexity-metrics-coupling-cohesion-and-hierarchical-depth)
     3. [Insights into Overall Structure and Organization:](#insights-into-overall-structure-and-organization)
     4. [Understanding Interactions Between Features:](#understanding-interactions-between-features)
   - [Object-oriented Design Measures:](#object-oriented-design-measures)
     1. [Beneficial for Object-oriented Approach:](#beneficial-for-object-oriented-approach)
     2. [Visual Representation with Class Diagrams:](#visual-representation-with-class-diagrams)
     3. [Measuring Class Size, Coupling, Inheritance Hierarchy, and Cohesion:](#measuring-class-size-coupling-inheritance-hierarchy-and-cohesion)
     4. [Understanding Encapsulation, Inheritance, and Polymorphism:](#understanding-encapsulation-inheritance-and-polymorphism)

## Onboarding:

### User Information and Preferences
- Farmer enables access to their location.
- Farmer enables access to their camera.
- Farmer selects preferred language during initial setup.

### Crop Selection and Size Input
- Farmer specifies the crop they are growing.
- Farmer inputs the size of the crop they are cultivating.

## Guide The User Page (Homepage):

### Today's Todos and Weather
- Displays a card with today's tasks (todos) and includes a weather widget.
  
### Latest Developments
- Provides a card with the latest developments relevant to the user's selected crop.

### Current Market Price
- Shows a card with the current market price of the selected crop.

### Reminder for Journal Entry
- Contains a card reminding the user to input journal entries such as rainfall, water content, pH content, and fertilizer amount sprayed.

## Features on Separate Pages:

### 1. Chat Room
- Allows users to connect with farmers growing similar crops.

### 2. Calendar
- Enables users to manage and edit their schedules, ensuring completion of tasks.

### 3. Journal
- Contains historical and present crop-specific information, including labor usage, yield during harvest, selling price, and daily measures such as water content and fertilizer amount.
- Includes a sub-feature to input information based on text from a notebook.

### 4. Insights and Recommendations
- Provides insights and recommendations based on journal information, industry averages, and scientific expected averages.
- Includes a sub-feature to identify crop diseases; uncertain cases are posted in group chats.

### 5. Autopilot Farming
- Enables setting up IoT devices and communication with the website.
- Automatically updates the journal daily and optimally plans activities based on weather forecasts.
- Makes intelligent decisions based on journal values and recommendations.
- Utilizes machine learning models in the background.
## Software Reviews:
- Architecture reviews
- Design reviews
- Code reviews

## Simulation and Prototyping:
- Simulation and prototyping can be conducted using tools like:
  - Mockup tools (e.g., Figma, Sketch) for user interface design.
  - Simulation software for testing algorithms and predictive models.
  - Prototyping tools (e.g., InVision, Adobe XD) for interactive demonstrations.

## Measures for Software Assessment:

### Function-based (Structured) Design Measures:

1. **Analyzing Functional Decomposition:**
   - Example:
     - Breaking down the application into manageable components such as:
       - Dashboard module
       - Chat room module
       - Calendar module
       - Journal module
       - Insights and recommendations module
       - Autopilot farming module
     - Each module focuses on specific functionalities related to its purpose, facilitating easier management and understanding of the system.

2. **Measuring Module Size, Complexity Metrics, Coupling, Cohesion, and Hierarchical Depth:**
   - Example: 
     - The dashboard module may have submodules for displaying weather information, market prices, and reminders.
     - Measuring the size (e.g., lines of code), cyclomatic complexity, coupling (dependencies between modules), cohesion (how closely related functionalities are grouped), and hierarchical depth of these submodules provides quantitative insights into their characteristics and relationships.

3. **Insights into Overall Structure and Organization:**
   - Example: 
     - Analyzing the structure of the dashboard reveals how different components (cards for todos, weather, developments, market prices, reminders) are organized and interconnected.
     - Understanding this structure helps in optimizing the layout for better user experience and maintainability.

4. **Understanding Interactions Between Features:**
   - Example:
     - Analyzing how changes in the journal module (e.g., adding new data entry fields) may affect the insights and recommendations module (e.g., adjusting recommendations based on new data) highlights the dependencies between different features.
     - This understanding guides the development process and ensures that changes in one component are properly reflected in others.

### Object-oriented Design Measures:

1. **Beneficial for Object-oriented Approach:**
   - Example:
     - Representing each module and its subcomponents as classes and objects (e.g., Dashboard, WeatherWidget, MarketPriceCard) facilitates a modular and scalable design.
     - This approach aligns well with the object-oriented paradigm, enabling better organization, encapsulation, and reusability of code.

2. **Visual Representation with Class Diagrams:**
   - Example:
     - Drawing class diagrams for modules like the journal, with classes representing data entry fields, methods for data processing, and relationships between classes (e.g., composition for encapsulating related data).
     - These diagrams provide a clear visual representation of the application's structure, aiding in design discussions and documentation.

3. **Measuring Class Size, Coupling, Inheritance Hierarchy, and Cohesion:**
   - Example:
     - Analyzing the journal module's class hierarchy reveals the inheritance relationships between classes (e.g., JournalEntry, JournalAnalyzer).
     - Measuring class size (number of attributes/methods), coupling (dependencies between classes), cohesion (how well-related functionalities are grouped within a class), and inheritance hierarchy depth provides insights into the design quality and maintainability of the module.

4. **Understanding Encapsulation, Inheritance, and Polymorphism:**
   - Example:
     - Encapsulating data and functionality within classes (e.g., encapsulating journal entry data within a JournalEntry class) ensures data integrity and promotes modularity.
     - Leveraging inheritance to create specialized classes (e.g., different types of journal entries inheriting from a common base class) enhances code reuse and flexibility.
     - Utilizing polymorphism to allow different types of journal entries to be processed uniformly (e.g., using a common interface for analyzing various entry types) simplifies code maintenance and extension.


Given the nature of the application and its various features like chat rooms, calendar, journal, insights, and autopilot farming, both function-based and object-oriented design measures can 
complement each other. Using function-based measures to analyze the overall functionality and structure of the application, while object-oriented measures can provide detailed insights
into the design at the class and object level. Combining both approaches can offer a comprehensive understanding of the application's design and facilitate better decision-making during the
development process.

