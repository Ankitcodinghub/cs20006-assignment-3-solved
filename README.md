# cs20006-assignment-3-solved
**TO GET THIS SOLUTION VISIT:** [CS20006 Assignment 3 Solved](https://www.ankitcodinghub.com/product/software-engineering-cs20006-solved-5/)


---

📩 **If you need this solution or have special requests:** **Email:** ankitcoding@gmail.com  
📱 **WhatsApp:** +1 419 877 7882  
📄 **Get a quote instantly using this form:** [Ask Homework Questions](https://www.ankitcodinghub.com/services/ask-homework-questions/)

*We deliver fast, professional, and affordable academic help.*

---

<h2>Description</h2>



<div class="kk-star-ratings kksr-auto kksr-align-center kksr-valign-top" data-payload="{&quot;align&quot;:&quot;center&quot;,&quot;id&quot;:&quot;116657&quot;,&quot;slug&quot;:&quot;default&quot;,&quot;valign&quot;:&quot;top&quot;,&quot;ignore&quot;:&quot;&quot;,&quot;reference&quot;:&quot;auto&quot;,&quot;class&quot;:&quot;&quot;,&quot;count&quot;:&quot;2&quot;,&quot;legendonly&quot;:&quot;&quot;,&quot;readonly&quot;:&quot;&quot;,&quot;score&quot;:&quot;5&quot;,&quot;starsonly&quot;:&quot;&quot;,&quot;best&quot;:&quot;5&quot;,&quot;gap&quot;:&quot;4&quot;,&quot;greet&quot;:&quot;Rate this product&quot;,&quot;legend&quot;:&quot;5\/5 - (2 votes)&quot;,&quot;size&quot;:&quot;24&quot;,&quot;title&quot;:&quot;CS20006 Assignment 3 Solved&quot;,&quot;width&quot;:&quot;138&quot;,&quot;_legend&quot;:&quot;{score}\/{best} - ({count} {votes})&quot;,&quot;font_factor&quot;:&quot;1.25&quot;}">

<div class="kksr-stars">

<div class="kksr-stars-inactive">
            <div class="kksr-star" data-star="1" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="2" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="3" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="4" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="5" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
    </div>

<div class="kksr-stars-active" style="width: 138px;">
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
    </div>
</div>


<div class="kksr-legend" style="font-size: 19.2px;">
            5/5 - (2 votes)    </div>
    </div>
We need to develop a rudimentary railway reservation / booking system (somewhat like IRCTC Train Ticket Booking, but extremely scaled down in features). We present various stages of this development process leading finally to the specific tasks of the assignment.

1 Specification

This is the outline specification that has been acquired from the client.

1.1 Requirement Statement

The entities involved in the booking system design include:

• Station: Every Station is identified by its name. Booking is done between any two Stations.

• Railways: It is the Indian railways. It has a collection of Stations with pairwise distance between Stations known a priori. Naturally, there can be only one Railways, called IndianRailways, in the system.

• BookingClass: There are several BookingClasses for travel (as in Indian Railways fare classes explained). Each BookingClass has the following attributes:

– Name: Name of the BookingClass

– Seat / Berth: Whether the BookingClass provides sleeping berths or just seats. This will not change in future.

– AC / Non-AC: Whether BookingClass is air-conditioned or otherwise. This will not change in future. – # of Tiers: How many tiers exist in the coach for this BookingClass. This will not change in future.

• Booking: A Booking is requested with the following information:

– fromStation: Station from which the travel starts for the Booking. This is given by the name of the Station

– toStation: Station at which the travel ends for the Booking. This is given by the name of the Station

– bookingClass: BookingClass for the Booking

On request of a Booking, the same is processed and fare is computed based on the business logic given in Section 1.3. The Booking is then confirmed with PNR and other details on the output. PNR is serially allocated starting with 1.

– name: Name of the passenger

– aadhaar #: Aadhaar Number to be used as a unique ID

– gender: Gender of the passenger: male or female

– mobile #: Mobile number (optional)

– category: One of General, Ladies, Senior Citizen, Divyaang, Tatkal, Premium Tatkal

1.2 Assumptions

The following assumptions are made for the design:

• IndianRailways has a given set of Stations with distances known a priori. The list of Stations and distances between them are given as Master Data in Section 1.4. No new station can be added to the IndianRailways and distance between pair of stations do not change.

• No passenger information is considered for the Booking

1.3 Business Logic

The fare between a pair of stations for a booking class is determined through the following steps:

• Base Fare: The base fare between two stations is computed by multiplying the distance between the stations with the base fare for every KM of travel. The base fare applies to the Sleeper booking class.

• Final fare is rounded to the nearest integer.

• Passenger has no effect on the fare as it is being ignored for now.

1.3.1 Example

For a booking from Delhi to Mumbai:

By AC3Tier:

• Distance from Delhi to Mumbai = 1447km

• Base fare = 1447km * Rs. 0.5 / km =

• Loaded fare for AC3Tier = Rs. 723.50 * 1.75 = Rs. 1266.125

• After adding the AC surcharge, we get Rs. 1266.125 + Rs. 50 = Rs. 1316.125 = Rs. 1316/= (rounded)

By ACFirstClass:

• Distance from Delhi to Mumbai = 1447km

• Base fare = 1447km * Rs. 0.5 / km =

• Loaded fare for ACFirstClass = Rs. 723.50 * 3.0 = Rs. 2170.50

• After adding the AC surcharge, we get Rs. 2170.50 + Rs. 50 = Rs. 2220.50

• Finally, we levy the luxury tax to get Rs. 2220.50 * 1.25 = Rs. 2775.625 = Rs. 2776/= (rounded)

1.4 Master Data

1.4.1 Stations

IndianRailways has five stations, namely: Mumbai, Delhi, Bangalore, Kolkata, and Chennai. The distances between the stations are given below:

Station Distance Matrix

From

Station To Station

Mumbai Delhi Bangalore Kolkata Chennai

Distance in KM

Mumbai X 1447

Mumbai 981

Mumbai 2014

Mumbai 1338

Delhi X 2150

Delhi 1472

Delhi 2180

Bangalore X 1871

Bangalore 350

Kolkata X 1659

Distance between a pair of stations is symmetric

1.4.2 Booking Classes

IndianRailways has seven booking classes as follows – shown with their respective attributes:

Booking Class Matrix

Booking Class Name Fare Seat / AC # Luxury / Remarks

Load Berth of Ordinary

Factor Tiers

ACFirstClass AC 3.00 Berth Yes 2 Luxury AC 2 berth

(1A) First Class coupe

AC2Tier AC 2.00 Berth Yes 2 Ordinary AC 2 berth inside,

(2A) 2 Tier 2 berth on side

FirstClass First 2.00 Berth No 2 Luxury Non-AC 2 berth

(FC) Class coupe

AC3Tier AC 1.75 Berth Yes 3 Ordinary AC 3 berth inside,

(3A) 3 Tier 2 berth on side

ACChairCar AC 1.25 Seat Yes 0 Ordinary AC chairs

(CC) Chair Car

Sleeper Sleeper 1.00 Berth No 3 Ordinary Non-AC 3 berth inside,

(SL) 2 berth on side

SecondSitting Second 0.50 Seat No 0 Ordinary Bench seating

(2S) Sitting

• Seat / Berth &amp; AC / non-AC classification, and # of tiers will not change in future

2 Analysis of Specification

We first analyze the specifications to identify the classes and hierarchy for the design. We also try to extract possible constraints on the design.

• Class Railways should be a singleton and should contain the master data of stations and distances. The singleton should be constant as no station can be added and distances cannot be changed.

If multiple properties are used in organizing the hierarchy, then the model would need multiple inheritance. However, we do not want to use multiple inheritance for the associated complications and inefficiency. Rather, we would use single inheritance on the strongest property and use the rest as HAS-A with polymorphic value based on the leaf class.

Naturally, there can be two candidates for this as Fare Load Factor, # of Tiers, and Luxury / Ordinary are more like pure attributes and clearly not useful for hierarchy:

– AC or Non-AC: Air-condition leads to comfort level, and is not fundamental to travel. So this is a weak candidate.

– Seat or Berth: This is fundamental property for a rail travel. So this is a strong candidate.

The hierarchy should be extensible in future as new booking classes are added.

3 High Level Design

Based on the analysis, now we carry out the High Level Design (HLD) below for Classes, Interfaces, Constants, Statics, Exceptions, and overall design considerations.

3.1 Design Principles

• Flexible &amp; Extensible Design

– The design should be flexible. That is, it should be easy to change the changeable parameters (like base rate, load factor etc.) easily from the Application space. This should should not need re-building of the library of classes.

– The design should be extensible. That is, it should be easy to add new behaviour (classes) wherever indicated in the specification (like Booking Classes, Booking, Passenger, etc.). This should not require a re-coding of the existing applications.

• Minimal Design

– Only the stated models and behaviour should be coded. No extra class or method should be coded.

– Less code, less error principle to be followed.

• Reliable Design

– Reliability should be a priority. Everything should work as designed and coded.

– Data members, methods and objects should be made constant wherever possible.

– Parameters should be appropriately defaulted wherever possible

• Testable Design

– Every class should support the output streaming operator for checking intermittent output if needed.

– Every class should be tested with an appropriate test application for its unit functionality (Section 6.1).

– Test Applications (Section 6.2) and regression test suites should be designed for testing the application on (at least) the common scenarios of use.

3.2 Classes

• Class Station HAS-A name.

• Class Railways is a singleton called IndianRailways. It has a collection of the Stations and their mutual distances. IndianRailways is a constant object.

3.3 Interfaces

• Constructors / Destructors: Proper constructor and destructor for every class

• Copy Functions: Provide user-defined Copy Constructor and / or Copy Assignment Operator for a class if used in the design (should not be needed). Otherwise, block them.

• Provide output streaming operator for every class to help output process as well as debugging

• Class Station to have GetName() for accessing its name and GetDistance(.) to get distance to another station.

• Class Railways to have GetDistance(., .) to get distance between a pair of stations. It should also have proper interface for making it a singleton IndianRailways

• Class Booking to have ComputeFare() to implement the fare computation logic. Should it be virtual (polymorphic) for future extensions?

3.4 Constants

The following should be static constants in appropriate classes:

• Load Factors of various BookingClasses

• Base Fare Rate: Rs. 0.50 / km

• AC Surcharge: Rs. 50.00

• Luxury Tax: 25% on booking amount

3.5 Statics

• Class Railways to have sStations (list of stations) and sDistStations (distance between stations).

• Class BookingClasses to have load factors.

• Class Booking to have sBaseFarePerKM, sBookings (list of bookings done), sBookingPNRSerial (next available PNR), sACSurcharge, and sLuxuryTaxPercent

3.6 Errors &amp; Exceptions

• There is no error in input, processing, or output.

• No error or exception handling to be incorporated in the design for this assignment. However, structure the code flow well so that they can be incorporated later with minimal changes (adhering to the need of flexibility).

4 Low-Level Design

Based on the High Level Design (HLD), we now perform the Low Level Design (LLD). LLD makes use of the specific constructs and idioms of C++.

4.1 Design Principles

• Encapsulation

– Maximize encapsulation for every class

– Use private access specifier for all data members that are not needed by derived classes, if any. Use protected otherwise.

– Use public access specifier for interface methods and static constants and friend functions only.

• STL Containers

– Use STL containers (like vector, map, hashmap, list, etc.) and their iterators. Do not use arrays – Use iterators for STL containers. Do not use bare for loops.

• Pointers &amp; References

– Minimize the use of pointers. Use pointers only if you need null-able entities

– If you use pointer for dynamically allocated objects (should be minimized), remember to delete at an appropriate position.

– Use const reference wherever possible.

4.2 Design of Classes, Data Members &amp; Methods

This is left as an exercise in the assignment. Design based on the HLD and the principles and document well.

5 Implementation

After completing the LLD, we perform the coding (implementation). In this we adhered to a set of basic guidelines and code organization.

5.1 Basic Coding Guidelines

5.2 Code Organization

Ideally, the definition of every class (or hierarchy) should be put in a corresponding .h file with the static definitions and method implementations in the respective .cpp. The application should be in Application.cpp file. However, for simplicity, it would be acceptable if all the codes are put in the Application.cpp file with the application.

6 Test Plan

We also need to prepare a test plan to test the implementation at different stages of development so that better quality and productivity can be ensured. Variety of test processes are common. We shall follow two of these in the current assignment.

6.1 Unit Tests

For the purpose of understanding, in Section B we illustrate the test plan and test function for a few unit cases for the Fraction class we have developed in Assignment 2.

6.2 Application Test

After the units have been tested, we integrate them into the application and test various scenarios for the application. A sample test application was provided for the Fraction class in Assignment 2. However, since it was just a single class application, the application code looked pretty much like the unit test application code with the exception of the comparison with golden data.

Like the units, we again need to enumerate scenarios for the application in the test plan and write the application test.

In addition, a sample test application for booking is given in Section C with the expected output in Section C.1. Your codes should pass this test application too.

7 Tasks

The following tasks are to be completed for the assignment:

1. Design: Complete the HLD and the LLD. Document the salient points from your design in Design.txt. Follow the quality guidelines and design principles outlined above.

2. Implementation: Implement the LLD in C++ following the basic coding guidelines (Section A).

4. Testing: Implement unit test and application test codes and perform testing. For application testing, test with the application given in Section C as well as the application developed by you from the testplan.

5. Bundle and Submissions: Name and bundle your files as given in Section 8 and submit to Moodle.

8 Submission of Files

The following files must be submitted as a single ZIP file:

1. Documents.zip

(a) Design.txt: The design document stating the design details (especially LLD) with principles and guidelines followed

(b) Testplan.txt: The testplan document stating scenarios for unit tests (with golden output if needed) and the scenarios of the test application.

2. Source.zip:

(a) Source (.cpp) and header (.h) files for implementation. (b) Source (.cpp) and header (.h) files for test application.

(c) README file that describes the contents of every file in the Source.zip. Also, mention the compiler (with version, and compiler options, if any) that you have used.

3. Outputs.zip

(a) Output from the given test application (Section C)

(b) Output from the your test application developed from the test plan

• The output file can be generated by redirecting the output to a text file or by copy-paste from the console in a text file.

• There is no need to include the a.out file.

Every file (with the exception of program output) must have your name and roll number.

Design

Breakup [20]

Non-static &amp; static data members [4]

Non-static1 &amp; static member functions signatures [4]

friend function signatures [2]

Design of BookingClasses Hierarchy [10]

Implementation

Breakup [25]

Non-static &amp; static member functions [15]

Static data members [5]

friend function [5]

Test Planning

Breakup [20]

Unit Test Scenarios &amp; Goldens (Completeness of scenarios) [15]

Application Test Scenarios [5]

Testing

Breakup [15]

Unit Test Application (adherence to test plan)

Own Test Application (adherence to test plan) [7]

Output

On given Test Application (Section C) [5]

Output [3]

Quality of Design &amp; Implementation

Breakup Adherence to Design Protocols [20]

Singletons [3]

const-ness [3]

Coding Guidelines [5]

Extensibility &amp; Flexibity [4]

Code Comments [5]

1 Non-static include non-polymorphic as well as polymorphic member functions

A Coding Guidelines

It is advised to follow the guidelines below while coding:

• Use CamelCase for naming variables, classes, types and functions

• Every name should be indicative of its semantics

• Start every variable with a lower case letter

• Start every function and class with an upper case letter

• Use a trailing underscore ( ) for every non-static data member

• Use a leading ’s’ for every static data member

• Do not use any global variable or function (except main(), and friends)

• No constant value should be written within the code – should be put in the application as static

• Prefer to pass parameters by value for build-in type and by const reference for UDT

• Every polymorphic hierarchy must provide a virtual destructor in the base class

• Prefer C++ style casting (like static cast&lt;int&gt;(x) over C Style casting (like (int))

• Indent code properly

• Comment the code liberally and meaningfully

• Adopt more guidelines as you prefer. Try to document them

B Unit Testing Fraction Class

As an example of unit test, let us consider the Fraction class we have developed in Assignment 2. We illustrate the test for its one overloaded constructor (Fraction(int = 1, int = 1)) and operator+ only. For this we enumerate the different possible cases to test in a unit test plan.

B.1 Unit Test Plan for Fraction

We elucidate the unit test plan for constructor and add operator.

B.1.1 Test Scenarios for Construction of Objects

We consider the Fraction(int = 1, int = 1) constructor. The scenarios (including normalization, sign handling, and default) are:

• Normalization

1. Improper fraction in reduced form

2. Improper fraction in irreduced form

3. Proper fraction in reduced form

4. Proper fraction in irreduced form

5. Fraction 0 with arbitrary denominator

• Sign handling

1. Fraction with negative numerator

2. Fraction with negative denominator

3. Fraction with negative numerator &amp; denominator

• Default parameters

1. Fraction with only numerator

2. Fraction with no parameter

B.1.2 Test Scenarios for Addition Operator

We consider the overloaded add operator friend Fraction operator+(const Fraction&amp;, const Fraction&amp;). The scenarios are (considering the given constructor):

1. Add two fractions

2. Add a fraction with an integer

3. Add an integer with a fraction

Rest of the Fraction class can be tested by preparing a similar plan.

B.2 Unit Test Implementation for Fraction

For unit testing, we write a static function in the class that has this test code. In the application, we use the ’golden output’ for every test and compare for equality. If the expected output is not obtained, a message on test error is printed.

B.2.1 Fraction Class Code

Here is the relevant parts of the class including the static test function signature

#ifndef __FRACTION_HXX// Control inclusion of header files

#define __FRACTION_HXX

/************ C++ Headers ************************************/ #include &lt;iostream&gt;// Defines istream &amp; ostream for IO using namespace std;

/************ CLASS Declaration ******************************/ class Fraction { public:

// CONSTRUCTORS

// ————

Fraction(int = 1, int = 1);// Uses default parameters. Overloads to

// Fraction(int, int);

// Fraction(int);

// Fraction();

// BINARY ARITHMETIC OPERATORS USING FRIEND FUNCTIONS // ————————————————-friend Fraction operator+(const Fraction&amp;, const Fraction&amp;); // Other member functions, static functions, friend functions // …

// STATIC UNIT TEST FUNCTION // ———————–static void UnitTestFraction(); // Test application for Fraction

// Data members

// …

#endif // __FRACTION_HXX

B.2.2 Fraction Class Unit Test Application Code

// To unit test class Fraction void Fraction::UnitTestFraction() {

// Check difference cases of fraction construction

Fraction f1(5, 3); // Improper fraction in reduced form

Fraction f2(15, 9); // Improper fraction in irreduced form

Fraction f3(3, 5); // Proper fraction in reduced form

Fraction f4(9, 15); // Proper fraction in irreduced form

Fraction f5(0, 2); // Fraction 0 with arbitrary denominator

Fraction f6(-2, 3); // Fraction with negative numerator

Fraction f7(2, -3); // Fraction with negative denominator

Fraction f8(-2, -3); // Fraction with negative numerator &amp; denominator

Fraction f9(5); // Fraction with only numerator

Fraction f10; // Fraction with no parameter

// Check if every object is constructed in the desired way if (f1.iNumerator_ != 5 || f1.uiDenominator_ != 3) // Check members cout &lt;&lt; “Fraction Consturction Error on Fraction(5, 3)” &lt;&lt; endl;

if (f2.iNumerator_ != 5 || f2.uiDenominator_ != 3) // Check members &amp; reduction cout &lt;&lt; “Fraction Consturction Error on Fraction(15, 9)” &lt;&lt; endl;

if (f3.iNumerator_ != 3 || f3.uiDenominator_ != 5) // Check members cout &lt;&lt; “Fraction Consturction Error on Fraction(3, 5)” &lt;&lt; endl;

if (f4.iNumerator_ != 3 || f4.uiDenominator_ != 5) // Check members &amp; reduce cout &lt;&lt; “Fraction Consturction Error on Fraction(9, 15)” &lt;&lt; endl;

if (f5.iNumerator_ != 0 || f5.uiDenominator_ != 1) // Check members with denominator = 1 cout &lt;&lt; “Fraction Consturction Error on Fraction(0, 2)” &lt;&lt; endl;

if (f6.iNumerator_ != -2 || f6.uiDenominator_ != 3) // Check members cout &lt;&lt; “Fraction Consturction Error on Fraction(-2, 3)” &lt;&lt; endl;

if (f7.iNumerator_ != -2 || f7.uiDenominator_ != 3) // Check members &amp; sign flip cout &lt;&lt; “Fraction Consturction Error on Fraction(2, -3)” &lt;&lt; endl;

if (f8.iNumerator_ != 2 || f8.uiDenominator_ != 3) // Check members &amp; sign flip cout &lt;&lt; “Fraction Consturction Error on Fraction(-2, -3)” &lt;&lt; endl;

if (f9.iNumerator_ != 5 || f9.uiDenominator_ != 1) // Check default on second parameter cout &lt;&lt; “Fraction Consturction Error on Fraction(5)” &lt;&lt; endl;

if (f10.iNumerator_ != 1 || f10.uiDenominator_ != 1) // Check default on both parameters cout &lt;&lt; “Fraction Consturction Error on Fraction” &lt;&lt; endl;

// Check addition of two fractions

Fraction f11 = f1 + f3; // Add two fractions

Fraction f12 = f1 + 1; // Add a fraction with an integer Fraction f13 = 1 + f3; // Add an integer with a fraction

if (f11.iNumerator_ != 34 || f11.uiDenominator_ != 15) // Check members on add cout &lt;&lt; “Fraction Addition Error on Fraction(5, 3) + Fraction(3, 5)” &lt;&lt; endl;

if (f12.iNumerator_ != 8 || f12.uiDenominator_ != 3) // Check members on add cout &lt;&lt; “Fraction Addition Error on Fraction(5, 3) + 1” &lt;&lt; endl;

if (f13.iNumerator_ != 8 || f13.uiDenominator_ != 5) // Check members on add cout &lt;&lt; “Fraction Addition Error on 1 + Fraction(3, 5)” &lt;&lt; endl;

return;

}

C Test Application for Booking

// Test application for booking void BookingApplication() {

// Bookings by different booking classes

// &lt;BookingClasses&gt;::Type() returns the constant object of the respective type

// Output the bookings done where sBookings is the collection of bookings done vector&lt;Booking*&gt;::iterator it; for (it = Booking::sBookings.begin(); it &lt; Booking::sBookings.end(); ++it) { cout &lt;&lt; *(*it);

}

return;

} int main() {

BookingApplication();

return 0;

}

Your implementation of classes needs to compile with the above application and output details of every booking done. A sample output could look as follows. It is not necessary to match every line of the output. But the same information should be available in your output.

C.1 Test Output

BOOKING SUCCEEDED:

PNR Number = 1

From Station = Mumbai To Station = Delhi

Travel Class = AC First Class

: Mode: Sleeping

: Comfort: AC : Bunks: 2

: Luxury: Yes Fare = 2776

BOOKING SUCCEEDED:

PNR Number = 2

From Station = Kolkata

To Station = Delhi

Travel Class = AC 2 Tier

: Mode: Sleeping

: Comfort: AC

: Bunks: 2

: Luxury: No

Fare = 1522

BOOKING SUCCEEDED:

PNR Number = 3

From Station = Mumbai

To Station = Kolkata

Travel Class = First Class

: Mode: Sleeping

: Comfort: Non-AC

: Bunks: 2

: Luxury: Yes Fare = 2518

BOOKING SUCCEEDED:

PNR Number = 4

From Station = Mumbai

To Station = Delhi

Travel Class = AC 3 Tier

: Mode: Sleeping

: Comfort: AC

: Bunks: 3

: Luxury: No Fare = 1316

BOOKING SUCCEEDED:

PNR Number = 5

From Station = Chennai

To Station = Delhi

Travel Class = AC Chair Car

: Mode: Sitting

: Comfort: AC

: Bunks: 0

: Luxury: No Fare = 1413

BOOKING SUCCEEDED:

PNR Number = 6

From Station = Chennai

To Station = Kolkata

Travel Class = Sleeper

: Mode: Sleeping

: Comfort: Non-AC

: Bunks: 3

: Luxury: No Fare = 830

BOOKING SUCCEEDED:

PNR Number = 7

From Station = Mumbai

To Station = Delhi

Travel Class = Second Sitting

: Mode: Sitting

: Comfort: Non-AC

: Bunks: 0

: Luxury: No

Fare = 362

BOOKING SUCCEEDED:

PNR Number = 8

From Station = Delhi

To Station = Mumbai

Travel Class = Second Sitting

: Mode: Sitting

: Comfort: Non-AC

: Bunks: 0

: Luxury: No

Fare = 362

The above test application is given as a sample. In addition, you should write your own unit and application tests.

D Clarifications

D.1 HAS-A relationship

A HAS-A relationship simply means having a component of an object (part of object) – it is Composition or Aggregation. It translates to having data members. For example,

Car HAS_A Registration_Number

Car HAS_A Engine

Car HAS_A Model_Name

Car HAS_A Wheel // 4 wheeler

Car HAS_A Owner

Wheel HAS_A SerialNumber

Wheel HAS_A Make

Wheel HAS_A Radius

Engine HAS_A Number

Engine HAS_A Capacity // in cc is modeled as

class Engine { protected: // Engines could be specialized const string engineNumber_; // every engine has a unique number that cannot change const int capacity_; // every engine has a unique capacity that cannot change

};

class Wheel { protected: // Wheels could be specialized const string SerialNumber_; // every wheel has a unique serial number that cannot change

const string&amp; make_; // Every wheel has a make that can be from a set of known makers

// Hence, reference to static maker names should be used

// Make cannot change

const double radius_; // Radius cannot change

};

class Car { protected: // Cars could be specialized const string registrationNumber_; // Registration number cannot change const Engine engine_; // Engine cannot change

const string&amp; modelName_; // Every car has a model that can be from a set of

// known models. Hence, reference to static model

// names should be used. Model cannot change

// make / radius

string&amp; ownerName_; // Owner can change for re-sale

}

We should not use private inheritance for HAS-A.

Note: Besides showing HAS-A, the above example also illustrates different situations for const-ness and reference

D.2 Private Inheritance

Note the following from the presentation:

• Private inheritance means nothing during software design, only during software implementation

• Private inheritance means is-implemented-in-terms of. It is usually inferior to composition, but it makes sense when a derived class needs access to protected base class members or needs to redefine inherited virtual functions

• It is good for enforcing a policy over a hierarchy. For example the following example of an uncopyable base class, which can be used to disable the copy constructor and assignment operator in derived classes:

class Uncopyable { protected:

Uncopyable() {}

~Uncopyable() {}

private:

Uncopyable(const Uncopyable&amp;);

Uncopyable&amp; operator=(const Uncopyable&amp;);

}; class Derived : private Uncopyable { … };

We should not use private inheritance unless we really need it. It is usually rare for most projects.

D.3 Virtual Destructor

The guidelines have the following:

Every polymorphic hierarchy must provide a virtual destructor in the base class This has attracted the following observation:

An abstract base classes cannot have a constructor or a destructor. So does this mean that this guideline is redundant?

So let us try to understood an Abstract Base Class better. It is a base class which has at least one pure virtual function. That’s it. And hence we cannot instantiate it; but we can always construct objects of it.

In any hierarchy, we must first construct the base class object before we can construct the derived class object (reverse for the destructor). So all classes concrete or abstract, must have constructor and destructor (which either you provide or get free from the compiler). A class is Abstract means that we cannot have an instantiation for it. But it will always get constructed and destructed as a base part of the derived class.

Finally, if the destructor is not virtual in a polymorphic hierarchy, then the destruction will not get dynamically dispatched to the derived class destructor and slicing will result. Let us look at the example below:

#include &lt;iostream&gt; #include &lt;string&gt; using namespace std;

class Base { const int id_; static int sObjId;

protected:

Base() : id_(sObjId++) { cout &lt;&lt; “Base Constructor for object id = ” &lt;&lt; id_ &lt;&lt; ” “; }

public:

virtual ~Base(); // Line 1 //virtual ~Base() = 0; // Line 2 virtual string GetName() const = 0; // Pure virtual function

int GetId() const { return id_; }

};

Base::~Base() { cout &lt;&lt; “Base Destructor for object id = ” &lt;&lt; id_ &lt;&lt; ” “; }

class DerivedOne : public Base { const string name_;

public:

DerivedOne(const string&amp; name) : Base(), name_(name) { cout &lt;&lt; “DerivedOne Constructor “; }

~DerivedOne() { cout &lt;&lt; “DerivedOne Destructor “; }

string GetName() const { return “DerivedOne: ” + name_ + ” “; }

};

class DerivedTwo : public Base { const string name_;

public:

DerivedTwo(const string&amp; name) : Base(), name_(name) { cout &lt;&lt; “DerivedTwo Constructor “; }

~DerivedTwo() { cout &lt;&lt; “DerivedTwo Destructor “; }

string GetName() const { return “DerivedTwo: ” + name_ + ” “; } }; int Base::sObjId = 0;

int main() {

//Base b; // Line 3: Does not compile – Base is abstract

const Base *p = new DerivedOne(“obj1”); cout &lt;&lt; p-&gt;GetName();

const Base *q = new DerivedTwo(“obj2”); cout &lt;&lt; q-&gt;GetName();

delete q; delete p;

return 0;

}

Base Constructor for object id = 0

DerivedOne Constructor

DerivedOne: obj1

Base Constructor for object id = 1

DerivedTwo Constructor

DerivedTwo: obj2

DerivedTwo Destructor

Base Destructor for object id = 1 DerivedOne Destructor

Base Destructor for object id = 0

Now, in Line 1, remove the word virtual, and the output changes to:

Base Constructor for object id = 0

DerivedOne Constructor

DerivedOne: obj1

Base Constructor for object id = 1

DerivedTwo Constructor

DerivedTwo: obj2

Base Destructor for object id = 1

Base Destructor for object id = 0

Clearly, the destructors of DerivedOne and DerivedTwo are not getting called as the destructor of Base is non-polymorphic. This is called slicing, as we just chop off the the head of the object leaving the torso behind. Interestingly, we can make the destructor itself pure virtual as well in (comment Line 1 and un-comment Line 2), and still provide its implementation, and we will get correct output as above. Often that is the default way around to start a polymorphic hierarchy:

class Base { public:

virtual ~Base() = 0;

};

// Derived classes …

Hence, Every polymorphic hierarchy must provide a virtual destructor in the base class

D.4 Source Header File and Library Conventions

D.4.1 Source File

Every C++ (C) source file should have .cpp (.c) extension. Many compilers decide the language rules to apply based on the file extension.

So, we shall use .cpp only.

D.4.2 Header File

Every header file (C++ or C) should be .h because we should write C in C++ compilable manner. However, since a header file is included in some source/s, its extension really does not matter to the compiler. It is more for the readability of the program.

Historically, .hpp extension was used by some companies to mean a C++ header and distinguish from a C .h header. These are legacy now. Some companies, in keeping with .cxx, used .hxx too.

So, we shall use .h only.

Once-only Inclusion of Header Files: Enclose every project header file with CPP guards as follows:

// Start of “Station.h”

#ifndef _STATION_H

#define _STATION_H

// Header file codes

#endif //_STATION_H

// End of “Station.h”

// Start of “Railways.h”

#ifndef _RAILWAYS_H

#define _RAILWAYS_H

#include “Station.h”

// Header file codes

#endif //_RAILWAYS_H

// End of “Railways.h”

Now when we include, say in, Booking.cpp as:

// Start of Booking.cpp

#include “Station.h”

#include “Railways.h”

// Source file codes

// End of Booking.cpp

the second inclusion of Station.h through Railways.h is excluded by the CPP guards. Otehrwise, we shall face re-definition errors.

In the C and C++ programming languages, #pragma once is a non-standard but widely supported pre-processor directive designed to cause the current source file to be included only once in a single compilation. It is better to avoid it (and use the scheme given above) for better portability.

D.4.3 Include Library

We have to be, however, more careful when we use the include library names as explained below:

• C++ Standard Library Headers: Include a C++ standard library header by name within angle brackets (&lt;&gt;):

#include &lt;iostream&gt; using namespace std;

All symbols are within the std namespace.

With angle brackets (&lt;&gt;), the header will be searched in the C++ standard library path defined in the system.

• C Standard Library Headers: In a C++ source, include a a C standard library header by name within angle brackets after prefixing it with c and dropping the .h. So stdio.h is included as:

#include &lt;cstdio&gt; using namespace std;

All symbols are again within the std namespace.

With angle brackets (&lt;&gt;), the header will be searched in the C++ / C standard library path defined in the system. cstdio is actually the C++ version of stdio.h.

In a pure C source (that will be compiled as C), include a C standard library header by name (with .h extension) within angle brackets (&lt;&gt;). So stdio.h is included as:

#include &lt;stdio.h&gt;

All symbols are within the global namespace.

With angle brackets (&lt;&gt;), the header will be searched in the C standard library path defined in the system.

Never include a C standard library header in C++ as the .h version

• Project Headers: Include a project header by name within a pair of double quotes (“”):

#include “Railways.h”

The symbols will be in the global namespace or the namespaces defined in the project headers.

With double quotes (“”), the header will be searched in the project path defined for the project.

D.5 static, const, Reference &amp; Singleton

• What should be Singleton?

There are several singletons on the project including the IndianRailways, BookingClasses etc.

• What should be the access specifier?

Always use private for data members, protected for data members needed by the inherited classes, and public otherwise. Constructor and Destructor should be private for singletons.

• What should be static?

Any object that should be available from the beginning to the end of the program, should be a static. Examples are collection of Stations, distances between Stations etc.

• What should be const? A value / object, by default, should be const unless it needs to change during the computation.

– What should be const value member?

A value / object that cannot change after the construction of an object. Like name of a Station etc. It is constructed / destructed with the object.

– What should be const reference member?

A value / object that cannot change after the construction of an object and refers to an object thatis defined (constructed / destructed) by some other object already.

– What should be const member function?

By default every member function should be const. Make it non-const if it is needed to change values and / or consider mutable to selectively change only a few data members in an otherwise const object. const-ness should be treat more semantically than syntactially. For more details check Section D.6.3

• What should be the access specification?

– private / protected: All data members, static or non-static, should be protected for a base class and private otherwise. Constructor / Destructor etc. should be protected for a singleton that is a base class, and private otherwise.

– public: All interface methods need to be public.

D.6 A Few Simple Design Principles

D.6.1 Class Members

In the same line, we should make name a private member of, say, class Station like const string name ;

• Yes, it is good to block copy functions (by providing them in private) if you do not need them so that in case they are used, you will get a compilation error. Note that in most contexts you should be using call/return-by-reference for UDTs (and call-/return-by-value for built-in types) and hence you would rarely need copying. Define properly when you need.

D.6.2 Hierarchy Design

1. Healthcare Workers (HCWs)

2. Frontline Workers (FLWs). FLW is a generalization of HCW

3. Senior Citizens (SCs), that is age &gt; 59 years

4. Person with Co-Morbidity (PCMs), where age &gt; 44 years and has one of the following Co-Morbidity

• Diabetes

• Heart failure with hospital admission in the past one year

• Post-cardiac transplant

• Valvular heart disease

• End-stage kidney disease on haemodialysis

• Severe respiratory disease with hospitalisation in the last two years

• Primary immunodeficiency diseases

• HIV infection

• Angina and hypertension/diabetes on treatment • …

5. More conditions of Phase 3 …

Looking at the above, we can identify the following attributes:

1. Nature of Work: Non-Frontline, Frontline, and Healthcare

2. Age: Below 45, Between 45 and 59, and Above 59

3. Co-Morbidity: Some 20 odd types. For simplicity we take this as Boolean: Non-Co-Morbid and CoMorbid

4. Gender: Female and Male. It is natural to have some criteria in future on this.

5. State: States on India. It is natural to have some criteria in future on this.

It is easy to see that the attributes will be available in the population is a totally mixed manner and in total we have 3 × 3 × 2 × 2 = 36 possible combination classes (ignoring the explosive possibility of States). Question is – how do we put them in a hierarchy? Naturally, every class will multiply inherited these properties in some path or other. That would not be a hierarchical design, it will be an anarchy.

So we decide to rank the attributes by their uniqueness. Model single inheritance on one or two of them and keep the rest as pure attribute values to be taken care of in the member function algorithms. For example, if we consider age as the most priority attribute (as we do in many population-related applications), we shall end up in a chaos as HCW, FLW, and Non-FLW would all exist in all ages. So age is a bad choice as a primary.

Hence, for a proper hierarchy, we should look at the natural flow of the model. Here, we can easily see that HCW in (1) is most specialized, FLW in (2) is the next, and (3) onwards it is the non-FLW. So Nature of Work should be the primary hierarchy parameter. Next, we see that other attributes have no effect on HCW and FLW. So only non-FLW is to be classified further. Here (3) predominates the age rule. Finally the Co-Morbidity takes over. Going by this principle from the analysis, we get 9 concrete classes and 3 levels.

// General population

// Abstract Base Class

class Person { };

// Frontline Workers // (1) to (5)

class FLW : public Person { };

// Non-Frontline Workers // (2)

class nonFLW : public Person { };

// Healthcare Workers // (3) to (5)

class HCW : public FLW { }; // Senior Citizen. Age &gt; 59 // (1)

class SC : public nonFLW { };

// Mid-Age Citizen. Age &lt; 59 &amp; &gt; 44 // (3)

class MC : public nonFLW { };

class YC : public nonFLW { };

// Co-Morbidity // (5)

class CM : public MC { };

// NonCo-Morbidity // (4)

class nonCM : public MC { }; // (5)

We can make it more compact, if we remove class CM and class nonCM from the hierarchy and just treat co-morbidity as a boolean attribute. This gives us 7 concrete classes and 2 levels. Naturally, gender and state both are also treated as attributes and we do not consider them for the hierarchy design.

So, the thumb rule would be to rank the attributes for the computation model and use one or two of them to create a two or three level hierarchy (ISA). Rest of the attributes should remain as attributes (HAS-A).

D.6.3 Semantics of const-ness

We often get confused between different shades of const-ness and their treatment in software design. It can feature in a variety of different contexts including:

• Natural Constants [static const in library]: Like π, e, c, etc.

• Universal Constants [static const in library]: Like days of the week etc.

• Design Constants

– Value Constants: Values that are constant for

∗ Life time of a particular object in a particular execution of the software [const data member]: Like Basic Pay of an Employee

∗ Life time of all objects in a particular execution of the software [static const in application]: Like Month of Pay Computation

∗ Life time of all objects in every execution of the software in a period, but can periodically change [static const in application]: Like the rate of Dearness Allowance of Employees (changes every six months to a year)

∗ Life time of all objects in every execution of the software in a period, but can occasionally change

– a change which is likely to software version change [static const in library]: Like Pay Scales

#include &lt;iostream&gt; #include &lt;string&gt; using namespace std;

class Gender { const string name_; protected:

Gender(const string&amp; name) : name_(name) {} public:

virtual const string Print() const = 0;

};

class Male : public Gender { Male() : Gender(Male::sName) {} static const string sName;

public:

// Singleton of Male that represents the type Male static const Gender&amp; Type() {

return theObj;

} const string Print() const { return “I am a man”; }

};

class Female : public Gender { Female() : Gender(Female::sName) { } static const string sName;

public:

// Singleton of Female that represents the type Female static const Gender&amp; Type() {

return theObj;

}

const string Print() const { return “I am a woman”; }

};

// Names defined as static constants const string Male::sName = “Male”; const string Female::sName = “Female”;

class Person { const string name_; const Gender&amp; gender_;

public:

Person(const string&amp; name, const Gender&amp; gender) : name_(name), gender_(gender) {}

friend ostream&amp; operator&lt;&lt;(ostream&amp; os, const Person&amp; p) { os &lt;&lt; p.name_ &lt;&lt; ” says: ” &lt;&lt; p.gender_.Print() &lt;&lt; endl; return os;

}

};

int main() {

Person p1(“Ramen Bag”, Male::Type()); // Type constants by singleton Person p2(“Elisa Tang”, Female::Type()); // Type constants by singleton

cout &lt;&lt; p1; cout &lt;&lt; p2;

return 0;

}

—-Outputs:

Ramen Bag says: I am a man

Elisa Tang says: I am a woman

– Behavior Constant [const in code contexts]: Like const pointer, reference, member function etc. • Implementation Constants [static const in library / application]: Like array size

• … Constant:

D.6.4 Testing • Every class must be tested for all its functionality in the Unit Test. Hence, it is advisable to keep every class simple – catering to one or two core ideas of the design only. You’ll have more classes – each for every unique concept your design has. This is often better than having few complex classes.

• Application Test should test for all scenarios of intended use of the software. It is good to prepare an exhaustive test plan for the scenarios first and then code each into the application.

• Testing Abstract Class

How can we test an abstract class? We cannot instantiate and create objects for the same.

Usually, these can be tested using mock (dummy / fake) objects of classes created by (minimally) specializing the abstract class with minimal functionalities for the polymorphic methods. (How to unit test abstract classes: extend with stubs?)

D.6.5 Null-able • Null-able parameters can be used for parameters (in an interface) to keep provision for future expansion and / or optional behavior. Easiest way to implement it is to use pointer with NULL as default. For example,

// Using Pointer class Passenger { // … };

void DoBooking( // Parameters …, const Passenger* = NULL); // Nullable

Alternately, we could have a specific constant static object of the class (being passed as parameter) interpreted as null and use as default parameter value. For example,

// Using Reference class Passenger { // … public: static const Passenger nullPassenger; // Semantically treated as a null passenger

}; const Passenger Passenger::nullPassenger;

void DoBooking( // Parameters …, const Passenger&amp; = Passenger::nullPassenger); // Nullable

D.7 Sample: Representing an Undirected Weighted Graph

Here we show an example of how to represent a (fixed) weighed undirected graph. This will help understand various aspects of the design that have been highlighted above. Consider the following project files carefully. Try to build and check out.

D.7.1 Node.h

#ifndef __NODE_H

#define __NODE_H

// ***** Node class definition of a graph

// ***** Author: P P Das

// ***** Version: 1.0

// ***** Known bugs: None

// ***** C++ Standard Library Headers

#include &lt;iostream&gt; #include &lt;string&gt; using namespace std;

// Nodes of a weighted undirected graph class Node { const string name_;

public:

Node(const string&amp; n) : name_(n) {

#if _DEBUG cout &lt;&lt; “Node ” &lt;&lt; n &lt;&lt; ” created” &lt;&lt; endl; #endif // _DEBUG

}

#if _DEBUG

~Node() { cout &lt;&lt; “Node ” &lt;&lt; name_ &lt;&lt; ” destroyed” &lt;&lt; endl;

}

#endif // _DEBUG const string&amp; GetName() const throw() { return name_; }

friend ostream&amp; operator&lt;&lt;(ostream&amp; os, const Node&amp; s) { os &lt;&lt; s.name_; return os;

}

};

#endif // __NODE_H

D.7.2 Node.cpp

// ***** Node class implementation of a graph

// ***** Author: P P Das

// ***** Version: 1.0

// ***** Known bugs: None

// ***** Project Headers

#include “Node.h”

D.7.3 Graph.h

#ifndef __GRAPH_H

#define __GRAPH_H

// ***** Graph class definition

// ***** Author: P P Das

// ***** Version: 1.0

// ***** Known bugs: None

// ***** C++ Standard Library Headers

#include &lt;iostream&gt;

#include &lt;string&gt; #include &lt;map&gt; using namespace std;

// ***** Project Headers

#include “Node.h”

#include “Exception.h”

// Forward declaration class Node;

// Weighted undirected graph class Graph { Graph();

~Graph();

// List of nodes as name-node pairs static map&lt;const string, const Node*&gt; sNodes;

// List of weights as &lt;node, node&gt;-weight pairs static map&lt;pair&lt;const Node*, const Node*&gt;, int&gt; sWeights;

public:

// Singletone Graph static const Graph&amp; TheGraph() {

// Local static singletone object

// Gets instantiated on the first call // Gets cleaned up with other static objects after main() static const Graph theGraph;

return theGraph;

}

// Gets the weight between two nodes

;

;

};

#endif // __GRAPH_H

D.7.4 Graph.cpp

// ***** Graph class implementation

// ***** Author: P P Das

// ***** Version: 1.0

// ***** Known bugs: None

// ***** C++ Standard Library Headers

#include &lt;iostream&gt;

#include &lt;string&gt; #include &lt;map&gt; using namespace std;

// ***** Project Headers

#include “Graph.h”

#include “Exception.h”

// ***** static Definitions map&lt;const string, const Node*&gt; Graph::sNodes; map&lt;pair&lt;const Node*, const Node*&gt;, int&gt; Graph::sWeights;

// ***** Implementation of Graph Graph::Graph() {

sWeights[make_pair(sNodes[“A”], sNodes[“B”])] = 3; sWeights[make_pair(sNodes[“A”], sNodes[“C”])] = 2; sWeights[make_pair(sNodes[“B”], sNodes[“D”])] = 9; sWeights[make_pair(sNodes[“C”], sNodes[“D”])] = 7;

#if _DEBUG cout &lt;&lt; “Graph created” &lt;&lt; endl &lt;&lt; endl;

#endif // _DEBUG }

Graph::~Graph() {

// Cleans up the nodes created map&lt;const string, const Node*&gt;::iterator it; for (it = sNodes.begin(); it != sNodes.end(); ++it) delete it-&gt;second;

#if _DEBUG cout &lt;&lt; “Graph destroyed” &lt;&lt; endl;

#endif // _DEBUG

}

{

// Looks for a node with matching name map&lt;const string, const Node*&gt;::iterator it; for (it = sNodes.begin(); it != sNodes.end(); ++it) if (it-&gt;first == name) return it-&gt;second;

throw Bad_Node(“No node as ” + name);

}

{ int weight = 0; try {

// Get the nodes const Node* psNode = GetNode(srcName); const Node* pdNode = GetNode(dstName);

// Get the weight between the nodes if they are connected map&lt;pair&lt;const Node*, const Node*&gt;, int&gt;::iterator weight_it; weight_it = sWeights.find(make_pair(psNode, pdNode)); if (weight_it == sWeights.end()) { weight_it = sWeights.find(make_pair(pdNode, psNode)); if (weight_it == sWeights.end()) throw Bad_Edge(“No edge between ” + srcName + ” and ” + dstName);

} weight = weight_it-&gt;second;

} catch (Bad_Node&amp;) { throw;

}

return weight;

}

D.7.5 Exception.h

#ifndef __EXCEPTION_H

#define __EXCEPTION_H

// ***** Exception class definitions for the project

// ***** Author: P P Das

// ***** Version: 1.0

// ***** Known bugs: None

// ***** C++ Standard Library Headers

#include &lt;iostream&gt;

#include &lt;string&gt; #include &lt;exception&gt; using namespace std;

// My exception class class Exception : public exception { string message_;

public:

Exception(const string&amp; msg) : message_(msg) { } const char* what() {

return message_.c_str();

}

};

// Thrown for a missing node for a name class Bad_Node : public Exception { public:

Bad_Node(const string&amp; msg) : Exception(msg) { }

};

// Thrown for a missing edge between two nodes class Bad_Edge : public Exception { public:

Bad_Edge(const string&amp; msg) : Exception(msg) { }

};

#endif // __EXCEPTION_H

D.7.6 App.cpp

// ***** Test Application for Graph

// ***** Author: P P Das

// ***** Version: 1.0

// ***** Known bugs: None

// ***** C++ Standard Library Headers

#include &lt;iostream&gt;

#include &lt;string&gt;

#include &lt;map&gt; #include &lt;cassert&gt; using namespace std;

// ***** Project Headers

#include “Graph.h”

#include “Exception.h”

// Application wrapper of GetWeight to handle exceptions int GetLinkWeight(const string&amp; n1, const string&amp; n2) throw (Bad_Node, Bad_Edge) { int w = 0; try { w = Graph::TheGraph().GetWeight(n1, n2);

cout &lt;&lt; “Weight between ” &lt;&lt; n1 &lt;&lt; ” &amp; ” &lt;&lt; n2 &lt;&lt; ” is = ” &lt;&lt; w &lt;&lt; endl;

}

catch (Bad_Node&amp; bn) { cout &lt;&lt; bn.what() &lt;&lt; endl;

} catch (Bad_Edge&amp; bl) { cout &lt;&lt; bl.what() &lt;&lt; endl;

}

return w;

}

int main() {

// Test cases checking with golden output

// These will assert on mis-matched output on Debug Build

// All asserts will vanish in a Release Build and there will be no output

// Both nodes exist with weight given in the called order assert(3 == GetLinkWeight(“A”, “B”));

// Both nodes exist with weight given in reverse of the called order assert(3 == GetLinkWeight(“B”, “A”));

// Both nodes exist but are not connected assert(0 == GetLinkWeight(“B”, “C”));

// First node does not exist assert(0 == GetLinkWeight(“E”, “B”));

// Second node does not exist assert(0 == GetLinkWeight(“A”, “F”));

// Both nodes do not exist – first node to be reported assert(0 == GetLinkWeight(“G”, “H”)); cout &lt;&lt; endl;

return 0;

}

D.7.7 Output in Debug build ( DEBUG is on)

Note that debug messages are given to track creation and destruction of objects:

Node A created

Node B created

Node C created

Node D created

Graph created

Weight between A &amp; B is = 3

Weight between B &amp; A is = 3

No edge between B and C

No node as E

No node as F

No node as G

Node A destroyed

Node B destroyed

Node C destroyed

Node D destroyed

Graph destroyed

D.8 Queries

D.8.1 Suryam Arnav Kalra

Sir , I have some doubts in this assignment.

1. Section 3.2 : Sir , it is written that the class Station HAS-A name , class BookingClasses HAS-A loadFactor but sir since name is just a string and loadFactor is just a double value, do I have to create separate classes for name and loadFactor or do I simply define them as string and double in their respective classes?

2. Section 3.3 : Sir , it is written to block the copy functions so do I write them in private with no implementation?

3. Sir , for the unit tests do I have to create a unit test for each class with all it’s member functions / utilities tested ?

4. SIr , for the applications testing file what extra shall I add since the file given seems to cover all the possibilities that we want to test for this application ?

D.8.2 Yashica Patodia

I am having a confusion regarding the HAS-A portion of the assignment.

1. From what I understand, private inheritance of classes is a HAS-A relationship but a HAS-A relationship is not necessarily a private inheritance. Please correct me if I am wrong.

So here, my doubt is should ’name’ be a private attribute of class ’Station’ or should I make a class ’name’ and then do private inheritance. I am unable to understand how to implement a HAS-A relationship on properties.

D.8.3 Rajas Bhatt

I have the following clarifications related to Assignment 3 of CS20006

1. In section 3.2 it has been written that ”Class Station HAS-A Name”. In normal circumstances, this denotes aggregation. As covered in the class, aggregation can be done in multiple ways. However, I think that using a c++ string instead of a custom Name class should work here. I don’t know what will be better.

2. In section 3.2 it has been written that ”Booking should support Passenger as a NULL-able parameter for future extension”. What does this mean?

3. In many instances, HAS-A relationships have been mentioned. Do these denote simple aggregation or necessarily Private Inheritance as covered in the class?

4. Can we use .hpp files instead of .h files?

5. In section 3.3 , bullet 4, it has been said that Class station should have getDistance() to get the distance to any other station, but aren’t we implementing all distance calculation machinery in the Railways class?

6. While designing unit tests for each class, do we really need to have header files? I don’t think this is necessary at all.

7. I have decided to keep BookingClasses as an Abstract base class (having two virtual functions), which has two derived classes (Seat and Berth) and they have my actual classes (like ACChairCar) . But the design is such that attributes, like name, ac/non-ac must be kept in the BookingClasses class itself. Now, since the BookingClasses is abstract, while constructing an object for my ACChairCar class, I cannot assign the attributes name , ac/non-ac etc. What should I do?

D.8.4 Nakul Aggarwal

1. Sir, in the class Railways, why do we have to assign stations and pairwise-distances to static data members? If static data members are used then they will have to be non-const because they are to be changed upon instantiation of the singleton object. But at the same time keeping this constant information specific to the singleton instance of the Railways class in non-const attributes can be problematic. Can’t we simply use non-static–const–private data members (to store stations and pairwise-distances) as was illustrated in one of the lectures?

2. I have a doubt in one guideline (page 9): Every polymorphic hierarchy must provide a virtual destructor in the base class. The only polymorphic hierarchy that we have in this project is the booking-class hierarchy. In this hierarchy all the base classes are abstract; and abstract base classes cannot have a constructor or a destructor. So does this mean that this guideline is redundant or have I misinterpreted it?

D.8.5 Nisarg Upadhyaya

1. Regarding statics in the singleton class Railways: What is the reason for making sStations and sDistStations statics in the Railways class. The design requires the class to be a singleton. The data members (private or public) if made static can be accessed using the scope resolution operator. I am not sure about this but intuitively it feels wrong to allow such access for a singleton class. Shouldn’t the access to any method/attribute be using the name of the singleton class, i.e., Railways::IndianRailways.data or Railways::IndianRailways.func()

2. Regarding BookingClasses hierarchy: I couldn’t comprehend the line ”Rather, we would use single inheritance on the strongest property and use the rest as HAS-A with polymorphic value based on the leaf class” on page 4. I understand that we are trying to create a single/double level hierarchy of abstract base classes with the first level on the basis of Seat/Berth inheriting from the root BookingClasses followed by the classes for different tiers inheriting from the Berth class. Then we can create any singleton concrete booking class inheriting from a leaf class of the aforementioned hierarchy that matches the Seat/Berth and tier specification required by the concrete class. What is the part ”use the rest as HAS-A with polymorphic value based on the leaf class” trying to convey?

3. Regarding constants: Why have changeable parameters like load factors, base fare rate, etc. been made static constants? Under 3.1 Design Principles, it has been asked that it should be easy to change these parameters from the application space.

4. Regarding copy functions: Does blocking of copy function mean we explicitly set them as private or provide no implementation and only definition for the same?

5. Regarding testing: Separate source and header files are required only for application testing right? For unit tests, we can have a static unit test function for each class whose implementation can be provided in the implementation file along with the implementation of the class as done in the unit testing of Fraction class? Also, confirming that no output is required for the unit tests developed.

D.8.6 Ashutosh Kumar Singh

1. So when you say that we encode the attributes on the methods, it means that there does not have an explicit member variable for AC/Non-AC, luxury, etc., right? We just return an appropriate boolean value from the virtual functions isAC() or isLuxury() as the case is. Is this correct?

3. According to what I understood, ”golden output” means that it is the theoretical output that we feel is correct. Is this right or is there something more to it?

4. There are various initializations which are to be done, for example creating the IndianRailways object, then as it is said that ” it should be easy to change the changeable parameters (likebase rate, load factor etc.) easily from the Application space”, so does this mean that these static constants should be initialized in Application.cpp? What I was thinking of is to initialize all the changeable statics in Application.cpp and all the non-changeable statics in their respective .cpp files itself.

5. I wanted to know where should the function bodies for each unit test function for each class be kept. Should each unit test function be in the respective source file of the class, or should all of them be in a different file like something called UnitTests.cpp?

Also, sir how are the unit test functions to be executed? I thought of putting all the unit test functions in a single file like UnitTests.cpp as mentioned, and then write a temporary main function in that class and then call each unit test function one by one. Is this how it is done, or is there some other procedure that is followed?

D.8.7 Aryan Singh

1. I was going through the lectures of singleton class for implementing the Railways assignment. In that I noticed that we explicitly call delete Printer::printer();

So Sir is it a good practice to call the destructor at the end of Main() or we should ignore calling delete .

D.8.8 Yindukuri Jayanth Phani Sai

1. I would like to know whether we are supposed to implement tests manually or we are allowed to use frameworks like Google Test, Boost.Test etc For the Unit Test Implementations part of the Assignment 3. I felt that learning and working with new frameworks in C++ might be fun.

D.8.9 Deep Majumder

1. I really love languages with ”strong” compilers that statically detect a lot of bugs. My first ”real” language was Java and I used to be quite impressed by its strictness. That is until I found out about Rust, which eliminates memory errors (and seg-faults) statically. Also Kotlin – I really find it useful to interoperate with JVM based libraries, while having a stricter compiler.

PPD: I love strong (type-safe) compilers too. But they come with an efficiency cost. None of these languages match (or come even near) the efficiency of C++ which often is a critical issue. So C++ is being elevated in its type-safety through various generations of C++11, 14, 17, 20, 23.

But enough of ranting – I would like to discuss with you what I feel about Singletons (especially since I am using it quite a lot now). As you mentioned in class, Singletons have two uses – one for objects that should exist uniquely and otherwise for creating types with an identity. The first one is of course quite necessary – and while we need hacks like Meyer’s singleton to represent it properly, while in Java we simply make everything static, it is still okay.

PPD: I would disagree. Meyer’s singleton is not a hack. It is one of the most beautiful implementation of a singleton devoid of any runtime support and / or resource management wrappers (like Smart Pointers). Further, I would rather call types with an identity as type constants with behavior.

The other use, as you mentioned, is to represent things like days of the week with types and have a compiler guarantee. However, one problem I can see is that since C++ class hierarchies are essentially open, we can easily add a ”eight” day by subclassing it in our application code.

PPD: You are right. Refering to Gender example, we can try to subclass Male and / or Female. It cannot be done because the constructors are private. However, if they are written with less rigour (constructor in protected, it takes a parameter etc.), you would be able to sub-class MoonMale from Male and MoonFemale from Female into the applications space as follows:

#include &lt;iostream&gt; #include &lt;string&gt; using namespace std;

class Gender { const string name_; protected: Gender(const string&amp; name) : name_(name) {} public: virtual const string Print() const = 0;

}; class Male : public Gender { static const string sName;

protected: // Constructor moved to protected and provided with a defaulted parameter

Male(const string&amp; name = “”) : Gender(name.empty()? Male::sName: name) {} public:

static const Gender&amp; Type() { static const Male theObj; return theObj; } const string Print() const { return “I am a man”; }

}; class Female : public Gender { static const string sName;

protected: // Constructor moved to protected and provided with a defaulted parameter

Female(const string&amp; name = “”) : Gender(name.empty()? Female::sName: name) { } public:

static const Gender&amp; Type() { static const Female theObj; return theObj; } const string Print() const { return “I am a woman”; }

};

const string Male::sName = “Male”; const string Female::sName = “Female”;

class Person { const string name_; const Gender&amp; gender_;

public:

Person(const string&amp; name, const Gender&amp; gender) : name_(name), gender_(gender) {}

friend ostream&amp; operator&lt;&lt;(ostream&amp; os, const Person&amp; p) { os &lt;&lt; p.name_ &lt;&lt; ” says: ” &lt;&lt; p.gender_.Print() &lt;&lt; endl; return os;

}

};

// In Application class MoonMale : public Male {

MoonMale() : Male(MoonMale::sName) {} static const string sName;

public:

static const Gender&amp; Type() { static const MoonMale theObj; return theObj; } const string Print() const { return “I am a moon man”; }

};

// In Application

class MoonFemale : public Female {

MoonFemale() : Female(MoonFemale::sName) {} static const string sName;

public:

static const Gender&amp; Type() { static const MoonFemale theObj; return theObj; } const string Print() const { return “I am a moon woman”; }

};

// In Application const string MoonMale::sName = “MoonMale”; const string MoonFemale::sName = “MoonFemale”;

int main() {

Person p1(“Ramen Bag”, Male::Type());

Person p2(“Elisa Tang”, Female::Type());

Person mp1(“$__X9 @oo8”, MoonMale::Type()); Person mp2(“!__V7 ?zv6”, MoonFemale::Type());

cout &lt;&lt; p1; cout &lt;&lt; p2; cout &lt;&lt; mp1; cout &lt;&lt; mp2;

return 0;

}

#include &lt;iostream&gt; #include &lt;string&gt; using namespace std;

// Forward declarations needed for the typedef’s class Male; class Female;

class Gender { const string name_; protected Gender(const string&amp; name) : name_(name) {} public: virtual const string Print() const = 0;

// Types are hardcoded here typedef Male HumanMale; typedef Female HumanFemale;

};

class Male : public Gender { Male() : Gender(Male::sName) {} static const string sName;

public:

static const Gender&amp; Type() { static const Male theObj; return theObj; } const string Print() const { return “I am a man”; }

};

class Female : public Gender { Female() : Gender(Female::sName) { } static const string sName;

public:

static const Gender&amp; Type() { static const Female theObj; return theObj; } const string Print() const { return “I am a woman”; }

};

const string Male::sName = “Male”; const string Female::sName = “Female”;

class Person { const string name_; const Gender&amp; gender_;

public:

Person(const string&amp; name, const Gender&amp; gender) : name_(name), gender_(gender) {}

friend ostream&amp; operator&lt;&lt;(ostream&amp; os, const Person&amp; p) { os &lt;&lt; p.name_ &lt;&lt; ” says: ” &lt;&lt; p.gender_.Print() &lt;&lt; endl; return os;

}

};

int main() {

// You cannot generate these types in library space (Gender) namespace

Person p1(“Ramen Bag”, Gender::HumanMale::Type()); Person p2(“Elisa Tang”, Gender::HumanFemale::Type());

cout &lt;&lt; p1; cout &lt;&lt; p2;

return 0;

}

PPD: So we have something better, though hacky. That is the price for performance.

It is a silly thing to do and will never get past code review – but it is still a problem that the compiler potentially could have solved but did not. Inspired by the Java enum solution, I tried looking into C++ scoped enums (which came in as late as C++11). On the face of it, it looks okay:

enum class DayOfWeek { SUN, MON, TUE, WED, THU, FRI, SAT };

However, I found out that underneath scoped enums, is really an underlying integer data type (like regular enums). So we can use static cast and to a disastrous effect. Like: DayOfWeek apocalypse = static cast&lt;DayOfWeek&gt;(7). This is thoroughly dis-satisfying and insufficient.

As a comparison, the Haskell solution would be something like:

data Class = ACFirstClass | FirstClass

| ACThreeTier

| ACTwoTier

| Sleeper

| ACChairCar

| SecondSitting

class BookingClass a where

getName :: a -&gt; String getNumTiers :: a -&gt; Int isSitting :: a -&gt; Bool isAc :: a -&gt; Bool

getLoadFactor :: a -&gt; Double

The Java solution will be pretty similar, using an enum which implements an interface. Long story short the C++ solution, as far as I know, is quite clunky and not even bulletproof. So Sir, I would like to know if it is possible to make a better, safer solution to this problem in C++, perhaps using more advanced C++? Or are we stuck with this? Because although C++ doesn’t have the same language beauty of Haskell or Rust, it is still the industrial standard and I really need to know it well. So Sir, could you please help me out with this?

struct Day { explicit Day(int d) : val(d) {} int val;

};

struct Month { explicit Month(int m) : val(m) {} int val;

};

struct Year { explicit Year(int y) : val(y){} int val;

};

};

PPD: Now Month can have 12 valid choices only. Like as follows:

class Month { public:

static Month Jan() { return Month(1); } // functions returning all valid

static Month Feb() { return Month(2); } // Month values; see below for

… // why these are functions, not

static Month Dec() { return Month(12); } // objects

… // other member functions

private:

explicit Month(int m); // prevent creation of new

// Month values

… // month-specific data

};

PPD: So the above simple design style can be used to have type-specific constant values. However, our real need in the context are Type Constants with with Behavior. So I chose the solution I provided. But I would never claim that it is indeed the best solution and will look forward to having a better way in C++. Anyone who can educate me on it – I would simply love it.

D.8.10 Rajat Bachhawat

1. In section 5.2 Code Organization, it is mentioned that we have to create an ’Application.cpp’. Is this the same test application that we have to make for carrying out application testing as mentioned in Task 7.4 Testing? Or is this a separate .cpp file that we have to create with a proper text based interface to accept user input and make bookings?

D.8.11 Parth Jindal

1. I had some doubts about how to go about testing abstract classes.What I had in mind was to make a wrapper class for them and create its fake object and test the polymorphic methods in it. Any directions for the same sir?

PPD: Added a point under Testing (Section D.6.4) to explain.

2. Also from a design perspective,when and why should singleton classes have static data members associated with it.Is it only making things semantically sound or does it have an underlying computational meaning to it.

PPD: I think we have already discussed different aspects of Singleton and static in depth in the clarifications and in response to Deep. Please go through them.

D.8.12 Anurat Bhattacharya

1. I was facing a problem during unit testing of Abstract Base Classes.Abstract Base Classes cannot be directly instantiated since it has some pure virtual functions.So I googled about it.What I got is that I need to create a mock object inheriting from the abstract base class with minimal functionalities and use it only for testing. How to unit test abstract classes: extend with stubs?

So regarding a mock object,Do we need to override the pure virtual functions and make them return some default value and then test the already defined methods of the abstract Base class.Or is there any other method for Unit Testing of Abstract Base Classes without writing mock objects.

PPD: Added a point under Testing (Section D.6.4) to explain.
