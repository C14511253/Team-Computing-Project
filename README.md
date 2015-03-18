# Team-Computing-Project
Group I's Team Computing Project
/* 
--------------------------------
Team Computing Project CA
Luke Griffin and Connor Heaphy
Started: 04/03/2015
Finished:
--------------------------------
*/

//Prototype
void object_1(void);


//MotorB is right wheel
//MotorC is left wheel

task main()
{
	//When robot senses an object
	while ( SensorValue(sonarSensor) > 25)
	{
		motor[motorB] = 50;
		motor[motorC] = 50;	
		
		//Call function
		object_1();
	}//End while
	

}//End main()


void object_1(void)
{
	int line_count = 0;
	
	//Counts 4 lines to the first block
	while(line_count != 3)
	{
		motor[motorB] = 50;
		motor[motorC] = 50;
		
		if(SensorValue(lightSensor) < 45)
		{	
			wait1Msec(50);
			line_count = line_count + 1;
		}//End if

	}//End While
	
	
	while(line_count != 3)
	{
		motor[motorB] = 50;
		motor[motorC] = 50;
		
		if(SensorValue(lightSensor) < 45)
		{	
			wait1Msec(50);
			line_count = line_count + 1;
		}//End if

	}//End While

}//End imlement object1
