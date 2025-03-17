# Week10 Research and Reflection Journal

## Notes:Model-View-Controller (MVC) Pattern

### Overview

- MVC is a user interface design/architecture pattern
- Used for organizing code in applications
- Focuses on separating different parts of an application

### Main Components

#### 1. Model

- Contains business logic and data
- Handles:
  - Data storage
  - Data modification
  - Data creation
- Usually implemented using classes or enums
- Must be completely independent of the view
- Can get data from different sources (local storage or cloud)

#### 2. View

- Represents the user interface
- Shows data to users
- Provides interaction opportunities
- Should not store any data or state
- Like a mirror reflecting the model's data

#### 3. Controller

- Most critical part of MVC
- Acts as a mediator between Model and View
- Responsibilities:
  - Captures user actions
  - Updates the model
  - Receives model changes
  - Updates the view
  - Transforms data to be appropriate for the view

### How MVC Works

1. User interacts with the View
2. Controller captures these actions
3. Controller updates the Model
4. Model processes the data
5. Model notifies Controller of changes
6. Controller updates the View
7. View shows updated information to user

### Current Status in Development

- Still common in web development
  - Used in: Ruby on Rails, Django, Angular, Vue
- Less common in mobile development
  - iOS: Moving towards MVVM and SwiftUI
  - Android: Prefers MVVM approach
- Other variations exist:
  - MVP (Model-View-Presenter)
  - MVI (Model-View-Intent)

## Q & A

### What is the hardest/most challenging thing you had to do this week for DGL 104?

- The most challenging aspect this week was understanding the Model-View-Controller pattern, particularly how the three components work together and maintain separation.

### How did you overcome this challenge?

- I will try to overcome this challenge by learning real-world examples and
practicing in development. I think review the examples in different frameworks
and compare MVC to newer patterns like MVVM will help me to understand the conceptions of MVC.
