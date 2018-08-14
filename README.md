# DateAgreementAPI/EventOrganiserAPI

The purpose of the DateAgreementAPI is to aid in the agreement of a suitable date, or period of dates, in a calander between a group of people based on their individually submitted preferences. 

The API has a number of functions:

Func1 - Initialise (Required data is provided by one person, triggering the request for all member's preferences.)
Func2 - Receive Event Response (A member of the group submits their preferences, triggering a reminder to all other members to submit their own preferences.)
Func3 - Receive Final Event Response (The final member of the group submits their preferences, triggering the results to be generated and circulted to all members to see.) 

Func1
Input parameters:
1) A date range that could span a matter of months or just days
2) Number of days as an integer or timespan
3) A list of email addresses

Output parameters:
1)Automated email sent to each email address provided in the list, as an input to func1. The email will contain a HTML calander displaying the range of dates provided as an input.

Func2
Input parameters:
1) A set of lists containing dates from the range in func1
  a) 1 list containing available dates
  b) 1 list containing unavailable dates
  c) 1 list containing undecided dates

Output parameters:
Automated email sent to each email address provided in the list, as an input to func1. The email will notify everyone that a member of the group has selected their preferred dates.

Inputs of func3:
1) The same as func2

Outputs of func3:
1) A number of potential solutions based on the submitted preferences and the initial date range/timespan
2) Automated email detailing the results sent to each member of the group
