using System;
using System.Collections.Generic;
using System.Linq;
using System.Text;
using System.Threading.Tasks;
using AwesomeCalculator;
using NUnit.Framework;

namespace Test_project_19th_Sep_2019
{
    public class Class1
    {
        [Test]
        public void GetAddition_Input3point4and5point6_Returns9point0()
        {
            //Arrangedouble 
            double number1 = 3.4;
            double number2 = 5.6;

            double expectedResult = number1 + number2; Calc testCalc = new Calc(number1, number2);
            //Act 
            double actualResult = testCalc.GetAddition();
            //Assert 
            Assert.AreEqual(expectedResult, actualResult);
        }

        [Test]
        public void GetSubtraction_Input20_Input15_Returns5()
        {
            //Arrangedouble 
            int num1 = 20;
            int num2 = 15;

            double expectedResult = num1 - num2;

            Calc testCalc = new Calc(num1, num2);
            //Act 
            double actualResult = testCalc.GetSubtraction();
            //Assert 
            Assert.AreEqual(expectedResult, actualResult);
        }

        [Test]
        public void Multiplication_Input12_Input0_Returns0()
        {
            //Arrangedouble 
            int num1 = 12;
            int num2 = 0;

            double expectedResult = num1 * num2;

            Calc testCalc = new Calc(num1, num2);
            //Act 
            double actualResult = testCalc.GetMultiplication();
            //Assert 
            Assert.AreEqual(expectedResult, actualResult);
        }

        [Test]
        public void Multiplication_Input34point6andpoint2_Returns210point8()
        {
            //Arrangedouble 
            int num1 = 34;
            double num2 = 6.2;


            double expectedResult = num1 * num2;

            Calc testCalc = new Calc(num1, num2);
            //Act 
            double actualResult = testCalc.GetMultiplication();
            //Assert 
            Assert.AreEqual(expectedResult, actualResult);


        }
        [Test]
        public void Division_Input90_Input2_Returns45()
        {
            //Arrangedouble 
            int num1 = 90;
            int num2 = 2;


            double expectedResult = num1 / num2;

            Calc testCalc = new Calc(num1, num2);
            //Act 
            double actualResult = testCalc.GetDivision();
            //Assert 
            Assert.AreEqual(expectedResult, actualResult);
        }

        [Test]
        public void Division_Input0_Input58_Returns0()
        {
            //Arrangedouble 
            int num1 = 0;
            int num2 = 58;


            double expectedResult = num1 / num2;

            Calc testCalc = new Calc(num1, num2);
            //Act 
            double actualResult = testCalc.GetDivision();
            //Assert 
            Assert.AreEqual(expectedResult, actualResult);
        }
    }
}
