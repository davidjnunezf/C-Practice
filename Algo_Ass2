
#include <stdio.h> 

//Log Time Pow function
float LogPow(float x, int y) 
{ 
	float result = 1;
    if(y==0){
        return result;
    }
    
    else if(y > 0){
        
	while (y > 0) { 
		
		if(y%2==1) {
		result = result * x; 
		}
		y = y/2;
		x = x * x; 
	}
	
    }
    
    else if(y < 0){
        
       	while (y < 0) { 
		
		if((y*-1)%2==1) {
		result = result/x; 
		}
		y = y/2;
		x = x * x; 
	} 
	
    }
	return result; 
} 

//Linear Time Pow function
float Pow(float x, int y){
    
    float result=1;
    if(y==0){
        return 1;
    }
    else if (y>0){
    for(int i=0; i<y; i++){
        result=result*x;
    }
    }
    else if(y<0){
       for(int i=0; i>y; i--){
           result=result/x;
       } 
    }
    
    return result;
    
}

// Tester Method
int main() 
{ 
	float x=3;
	int y=-5;

	printf(" Linear time: pow(%2f, %2d) = %2f \n ",x,y,Pow(x, y));
	printf("lg n time pow(%2f, %2d) = %2f",x,y, LogPow(x, y)); 

	return 0; 
}
