<!doctype html>
<html>
    <head>

    </head>
    <body>
        <h1>
            &nbsp;&nbsp;&nbsp;&nbsp;&nbsp; &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
            &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;AGE CALCULATOR
        </h1>
        <br>
        <p><img src="images.png" width="225" height="225"> </p>
     </body>
</html>
<html>
   <head>
   <script>
       function ageCalculator() {
             var userinput = document.getElementById("DOB").value;
             var dob = new Date(userinput);
                    if (userinput == null || userinput == '') {
                        document.getElementById("message").innerHTML = "**Choose a date please!";
                        return false;
                    }


                    else {

                        var dobYear = dob.getYear();
                        var dobMonth = dob.getMonth();
                        var dobDate = dob.getDate();


                        var now = new Date();

                        var currentYear = now.getYear();
                        var currentMonth = now.getMonth();
                        var currentDate = now.getDate();


                        var age = {};
                        var ageString = "";


                        yearAge = currentYear - dobYear;


                        if (currentMonth >= dobMonth)

                            var monthAge = currentMonth - dobMonth;
                        else {
                            yearAge--;
                            var monthAge = 12 + currentMonth - dobMonth;
                        }


                        if (currentDate >= dobDate)

                            var dateAge = currentDate - dobDate;
                        else {
                            monthAge--;
                            var dateAge = 31 + currentDate - dobDate;

                            if (monthAge < 0) {
                                monthAge = 11;
                                yearAge--;
                            }
                        }

                        age = {
                            years: yearAge,
                            months: monthAge,
                            days: dateAge
                        };


                        if ((age.years > 0) && (age.months > 0) && (age.days > 0))
                            ageString = age.years + " years, " + age.months + " months, and " + age.days + " days old.";
                        else if ((age.years == 0) && (age.months == 0) && (age.days > 0))
                            ageString = "Only " + age.days + " days old!";

                        else if ((age.years > 0) && (age.months == 0) && (age.days == 0))
                            ageString = age.years + " years old. Happy Birthday!!";
                        else if ((age.years > 0) && (age.months > 0) && (age.days == 0))
                            ageString = age.years + " years and " + age.months + " months old.";
                        else if ((age.years == 0) && (age.months > 0) && (age.days > 0))
                            ageString = age.months + " months and " + age.days + " days old.";
                        else if ((age.years > 0) && (age.months == 0) && (age.days > 0))
                            ageString = age.years + " years, and" + age.days + " days old.";
                        else if ((age.years == 0) && (age.months > 0) && (age.days == 0))
                            ageString = age.months + " months old.";

                        else ageString = "Welcome to Earth! <br> It's first day on Earth!";


                        return document.getElementById("result").innerHTML = ageString;

                    }
                }
            </script>
        </head>
        <body>
            <center>
                <h2 style="color: 32a80f" align="center"> Calculate Age from Date of Birth <br> <br> </h2>

                <b> Enter Date of Birth: <input type=date id=DOB>  </b>
                <span id="message" style="color:red"> </span> <br><br>
                <button type="submit" onclick="ageCalculator()"> Calculate age </button> <br><br>
                <h3 style="color:32a80f" id="result" align="center"></h3>
            </center>
        </body>
    </html>
    <br>
<html>
<head> </head>
 <body>
    <ul>
        <li> <a href="#About me"> About me</a> </li>
        <li> <a href="#reason for this homepage"> motivation for making homepage </a> </li>


    </ul>
    <h4> ABOUT ME </h4>
    <br>
    <p>
        <a name="About me">
            Hey evryone,
            I am Surbhi Srivastava a 1st year undergraduate at IIT BOMBAY. <br>
            Mechanical engineering department dual degree program basically interested in learning programing languages. <br>
            my hobbies are eating ,sleeping, and <br>
            watching movies (although i don't get time for it now :( ).
            <br>
        </a>
    </p>
    <p>
        contact me at
        <ul>
            <li> <a href="https://www.facebook.com/surbhi.srivastava.10888/"> Facebook id </a> </li>
            <li> <a href="srivastava1801@gmail.com"> srivastava1801@gmail.com </a> </li>
        </ul>
    </p>
    <h3> This is me </h3>
    <p> <img src="me.jpeg" width="300" height="400"> </p>
    <br>
    <br>
    <br>
    <h4> MOTIVATION FOR MAKING HOMEPAGE </h4>
    <br>
    <p> <a name="reason for this homepage"> I have participated in SOC and as a part of this project <br> i am doing this to learn my weak was to rush with two upcoming quizzes its mid night saturdayy and i have to submit my assignment before 12 noon and i am loving it :) </a> </p>
 </body>
 
</html>
