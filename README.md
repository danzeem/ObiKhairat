# ObiKhairat (private project)

### *Bringing Transparency and Progress to charity giving in Malaysia*

## What will the application do ?
Obikhairat lets **trusted charity organizations** to upload their financial documents, such as monthly report, balance sheet, and cash flow statements.
Instead of blindly donating the money to a charity organisation and hoping they are going to do the real progess, so donors can view exactly where the money goes. 
Every registered organization has a public profile showing its uploaded documents. This gives transparency to the users to look at the financial report, before they decide to donate. 

## Who will use it?
 - **Malaysian donors** who want to give with confidence
 - **Trusted organisation** (ie. those who are backed by a government fund investment) who upload their reports to maintain public accountability

## Why is this project interests me 
- I've volunteered with charity organizations in Malaysia for **6 years**, and I have a growing frustation
watching NGOs to use most of their donation into short-term relied, such as food, and emergency aid, while very less goes toward long-term progress like 
education, or policy research. 
- Charities are everywhere in Malaysia. This will drive the cost while most of the organizers run the charities without real experties in economics, urban planning, or accounting.
- I want to build something that lets donors see the real picture, and pushes organizations toward the kind of transparency that earns long-lasting trust. 
- My hope is that one day, an app lke this cana hel people in my country give safely and actually see the change over the next 10 years. 
*User stories* : 
- As a user, I want to be able to see the organization’s financial details
- As a user, I want to be able to see the organization’s overview
- As a user, I want to be able to see the organization’s impacts made
- As a user, I want to donate to the organization I choose.
- As a user, I want to know how much I have donated since the account's inception.
- As a user, I want to be able to view the list of trusted organizations
- As a user, I want to be able to add a document to an organization's profile
- As a user, I want to be able to save the entire state of the app, including my donor
 profile and every registered organization, with their file document
- As a user, I want to be able to load the previously saved state from file, so I can 
resume with my donor profile and all organizations exactly as they were.

## Phase 4: Task 2

Sample console output printed when the application is quit:

Wed Jun 03 14:22:10 PDT 2026
Organization added to charity: Khazanah

Wed Jun 03 14:23:47 PDT 2026
User Alex donated $50 to Khazanah

Wed Jun 03 14:23:47 PDT 2026
Organization Khazanah received donation of $50 (total now $1000050)

## Phase 4: Task 3
If I had more time, I would refactor `CharityAppUI` so that it has fewer responsibilities. 
It currently manages the GUI screens and navigation while also storing important data such as the active user, 
charity, and organization. I would separate the application state into another class and let `CharityAppUI` focus mainly on controlling and displaying the GUI. 
This would improve cohesion because each class would have a clearer responsibility, 
and it would also reduce the coupling between the screen and the application's state.

I would also refactor some of the repeated behaviour in my `Screen` subclasses. Many screens use the same controller to navigate between screens, and several contain similar button and navigation logic. 
I could move some common navigation behaviour into the abstract `Screen` class or another helper class.
This would reduce duplicated code and make it easier to modify the GUI structure in the future without changing many individual screen classes. 
