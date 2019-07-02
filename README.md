# Unnamed-Nonprofit
Technical specs and wireframes of an idea-stage nonprofit for feedback.

Technical Specs - Unnamed Nonprofit 

July, 1, 2019  

Author: Madison Skov 

Contributors: Ryan Milbourne

# Overview

**General approach** - Reuse open source software to build a progressive web app off the core game component.  

**Estimated time to complete** - 4 Weeks

**Summary** - The proposed nonprofit seeks to covertly assist adult women in escaping abusive relationships and circumstances by providing one-way, one-time plane tickets towards a fresh start in a new city unknown to their abusers. The pool of cities for relocation are selected based on the collection resources available to survivors of abuse, with whom the Nonprofit coordinates on behalf of users to establish a growth and recovery plan. Resoursources sourced through local networks include housing, support groups, security education, psychological therapy, financial assistance, and job placement. Donations are accepted in fiat currency and bitcoin. Tickets are purchased by the nonprofit on behalf of users in either bitcoin or fiat depending on the price of the cheapest ticket for the city and date selected by the user. Among organizational features, the Nonprofit webpage contains educational informational on personal security, bitcoin and bitcoin wallets, and gig economy jobs which pay in both fiat and bitcoin. 

**Context** - View wireframes at [https://hcoiot.axshare.com](https://hcoiot.axshare.com)

# Goals 



1. Get users out
2. Highly covert with minimal demands placed on the user
3. Provide education for personal security and financial independence 

# Product Requirements 



*   Display of user account funds is password protected within the game
*   Long press (3-sec) to close game from any view
*   Lowest priced flights from user location are selected from pool of approved cities
*   View of funds in user account and Cash-out screen are personal password protected
*   Users flight details delivered to both the Nonprofit and local resources once the ticket is booked
*   Account terminated following flight departure time and date. Updates to flight status by the operating airline are made automatically so that premature termination does not occur. If refund is applicable in the case of a missed flight, funds are distributed among active accounts. 
*   Accounts of tickets not purchased for 3 months when cashout is available are terminated and funds accumulated are distributed among active accounts. 

# Assumptions



*   WOM will be sufficient for identifying and passing passwords to potential users
*   Funds will be managed by the np through a secure custodial platform
*   Users will be able to view the amount allotted for them, but not have access to the funds directly. Funds will be applied directly to purchasing a plane ticket.
*   Cities are selected relative to quality and number of relevant resource available and cost of flight. 
*   Users can earn bitcoin and deposit it directly into their account towards their ticket. 
*   The nonprofit lists accurate and detailed information, resources, and links to teach and assist users in increasing their personal and financial security. 
*   The nonprofit page also lists details on resources available by state and city to abuse survivors.
*   The nonprofit collects the user’s first name from the ticket transaction page other than the departure/arrival time/location in order to have the user collected at arrival by local organizations. The user may approach the local organization representative, or not if she chooses. 
*   Funds remaining in an account after ticket purchase will be redistributed among active accounts. 

# Out of Scope



*   User control of the donated bitcoin through the nonprofit directly
*   Ability to earn additional bitcoin directly through this nonprofit beyond what is contributed by donors 
*   Direct communication between users and nonprofit

# Approach



*   Hands-off, minimal solution passed by WOM only.  
*   Progressive Web App

   **Home** 

*   Accessing the game

  **Game**

*   Bejeweled
*   Built off Koji skin open source code
*   3-Second long press closes game on any screen

  **High Scores**

*   Lists scores
*   Play again
*   View your points

   **Points**

*   Jewel Points
*   password protected
*   Enter WOM password → change password to personal password → activates donation account in coinbase. 
*   Funds within account displayed as Jewel Points
*   Amount of funds needed until threshold for ticket purchase displayed
*   Personal password must be entered to display Jewel Points
*   When enough Jewel Points are reached, Cashout is accessible.
*   Number of each type of jewel matched in game viewable
*   Play again

   **Cashout**

*   One way, single person ticket
*   Cheapest flights from departing airport from a repository of cities with approved resources
*   Date and airport are selectable
*   Airline logo, city name, #stops, duration, and price are listed for each available flight

**Flight Information**


*   Lists resource information for given city
*   Back
*   Select - window opens incognito to the booking page for this flight with the designated airport and date autofilled 


   **NP’s Page**


 *   NP’s mission
 
 *   Get Help 
 
 *   Donation 
 
 *   Resources

   1. What and why bitcoin
   2. Wallets for new users
   3. How and where to earn
   4. User security prior to and following relocation

 *   News & Events 

 *   About
      
 *   Contact us

# Other Options Considered

Hidden wallet - no way to ensure users are indeed victims without risking compromising  their identities. Overly complex, not necessary for users who are not monitored digitally who have access to other options. 

	

# Components


*   Home 
*   Game
*   High Scores
*   Points (password protected)
*   Cashout
*   Flight Information
*   Link out to book flight
*   NP’s Page

# Schema 

[Schema architecture](https://imgur.com/iQqLdRO)


# Security and Privacy

Biggest risks:


*   Bad actors
*   Harm enacted on users who have been found out

# Test Plan



*   Manually test all important user stories

# Deployment and Rollout



*   Deploy infrastructure
*   Deploy donation website
*   Deploy game code

# Rollback Plan



*   Disable cashout until bugs fixed

# Metrics



*   Number of tickets purchased
*   Number of individuals received at arrival airport
*   Number of individuals who are safe a month after their flight

<!-- Docs to Markdown version 1.0β17 -->
