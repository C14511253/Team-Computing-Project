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
//MotorB is right wheel
//MotorC is left wheel

task main()
{
	int line_count = 0;		//Counts the number of lines passed over

	while(line_count != 4)
	{
		motor[motorB] = 50;
		motor[motorC] = 50;
		
		if(SensorValue(lightSensor) < 45)
		{	
			wait1Msec(50);
			line_count = line_count + 1;
		}//End if
		
	}//End While

}//End main()
