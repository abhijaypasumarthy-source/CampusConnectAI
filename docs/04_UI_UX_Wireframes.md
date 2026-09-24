# UI/UX & Wireframes

## 25. UI Wireframes Overview
The application will utilize a modern, minimalist design system. Primary colors: University Blue and Clean White.

## 26. Landing Page Design
*   **Hero Section:** 
    *   Headline: "Navigate Campus. Find Answers. Instantly."
    *   Subheadline: "Meet CampusConnect AI, your smart university assistant."
    *   Primary CTA: "Start Chatting" | Secondary CTA: "Open Map"
*   **Features Grid:** Icons + text highlighting Navigation, Faculty Search, AI Assistant, and Live Events.
*   **Footer:** University links, contact, admin login.

## 27. Dashboard Design (Student View)
*   **Top Nav:** Search Bar (Global), User Avatar, Notifications.
*   **Main Content Area:**
    *   **Left Column (60%):** Dynamic Map Snippet showing current location and "Quick Route" input boxes (From -> To).
    *   **Right Column (40%):** "Upcoming Events" list and "Important Notices" feed.
*   **Floating Action Button (FAB):** Persistent AI Chat icon in the bottom right corner.

## 28. AI Chat Interface Design
*   **Layout:** Similar to ChatGPT or standard messaging apps.
*   **Header:** "CampusConnect Assistant" with an online indicator.
*   **Chat Area:** 
    *   User messages on the right (Blue bubbles).
    *   AI messages on the left (Gray bubbles).
    *   AI responses can contain "Action Chips" (e.g., if AI says "Dr. Ramesh is in AB1-204", a chip below says `[Show on Map]`).
*   **Input Box:** Text input, microphone icon (for future speech-to-text), and a Send button.

## 29. Faculty Search Page
*   **Search Header:** Large input bar "Search by name, department, or subject..."
*   **Filter Sidebar:** Dropdowns for Department (CS, Mech, Bio) and Building.
*   **Results Grid:** Faculty cards containing:
    *   Photo & Name
    *   Designation & Department
    *   Cabin Room Number
    *   Button: `[Navigate to Cabin]`

## 30. Campus Navigation Page
*   **Full-Screen Map:** Interactive canvas showing the campus blueprint.
*   **Search Overlay (Top Left):**
    *   Input 1: "Current Location" (or select from list).
    *   Input 2: "Destination" (Room, Lab, Building).
*   **Route Info Panel (Bottom):** 
    *   Distance: 450m
    *   Estimated Time: 5 mins
    *   Step-by-step text directions: "1. Exit Main Gate -> 2. Turn left at Library -> 3. Enter AB2."
