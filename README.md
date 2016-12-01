Elevator Simulation Problem  
  
Edit only the function definition of Elevator.prototype.decide() in myelevator.js.  
That function is called when elevator needs to decide which floor it needs to go to.  
Try to:  
1. minimize total_people_wait_time_in_elevator  
2. minimize total_people_wait_time_out_elevator  
3. minimize total_elevator_traveled_distance  
4. maximize total_delivered_people  

#Explanation

1.  All elevator sweep through requests, if a request existed it will take the request if it's on the same direction as the elevator.
2.  If an elevator missed a request because it's already going up or going down, it search for another elevator.
3.  If there are no requests or tasks, it will park on the 15th floor.
4.  The statistic result show optimal number of people waiting outside (under 7k) but poor number on people wait time on elevator (beyond 10k), this caused by setting the elevator to take all the request while it's delivering people.
5.  I dont know if this is the most efficient, but I did my best. 
6.  Based on personal experience, I would rather wait inside the elevator rather than outside ;)
