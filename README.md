# Oystercard

This is our week 2 Makers challenge, do be worked on during afternoon pairing sessions.

I'm hoping to build ont he skills learned in week 1, and use TDD to build the program, with particular focus on learning how to:

Break one class into two classes that work together, while maintaining test coverage
Unit test classes in isolation using mocking
Explain some basic OO principles and tie them to high level concerns (e.g. ease of change)
Review another person's code and give them meaningful feedback
rspe
In order to use public transport
As a customer
I want money on my card

In order to keep using public transport
As a customer
I want to add money to my card

In order to protect my money
As a customer
I don't want to put too much money on my card

In order to pay for my journey
As a customer
I need my fare deducted from my card

In order to get through the barriers
As a customer
I need to touch in and out

In order to pay for my journey
As a customer
I need to have the minimum amount for a single journey

In order to pay for my journey
As a customer
I need to pay for my journey when it's complete

In order to pay for my journey
As a customer
I need to know where I've travelled from

In order to know where I have been
As a customer
I want to see to all my previous trips

In order to know how far I have travelled
As a customer
I want to know what zone a station is in

In order to be charged correctly
As a customer
I need a penalty charge deducted if I fail to touch in or out

In order to be charged the correct amount
As a customer
I need to have the correct fare calculated

\#touch_in
\@in_system = true

\#touch_out
\@in_system = fals

\#in journey
\@in_use

\#touch_in
balance check
\@in_system

\#touch_out
balance - Minimum value
\@in system

\#touch_in(station)
balance check
\@current_station = station
\@in system


In order to pay for my journey
As a customer
I need to know where I've travelled from

\@entry_station


In order to pay for my journey
As a customer
I need to know where I've travelled to

\@exit_station

In order to know where I have been
As a customer
I want to see to all my trip

{entry => \@after_entry, exit => \@exit_station}

In order to know where I have been
As a customer
I want to see to all my previous trips

[{@my_trip}, {@my_trip}, {@my_trip}]




In order to know how far I have travelled
As a customer
I want to know a station

\class Station

In order to know how far I have travelled
As a customer
I want to know the name of station is in
\station.name

In order to know how far I have travelled
As a customer
I want to know what zone a station is in

\station.zone


In order to be charged correctly
As a customer
I need a penalty charge deducted if I fail to touch in or out

Journey Class

\journey.start
\journey.end
\journey.complete?

\journey.calculate_fare
=> returns MINIMUM_FARE
=> if incomplete, returns PENALTY_FARE = 6


