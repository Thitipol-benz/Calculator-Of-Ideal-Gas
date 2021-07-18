#include <stdio.h>

double P,V,n,R,T,value,z;
main ()

	{
            int A;
            st:
            printf("\a");	
		    printf("***********************\n");	
			printf("++Ideal Gas Law++\n");
		    printf("--- PV = nRT ---\n");
		    printf("+++CALCULATOR+++\n");
		    printf("******MENU******\n");
            printf("Find P plesse select(1)\n");
            printf("Find V plesse select(2)\n");
            printf("Find n plesse select(3)\n");
            printf("Find T plesse select(4)\n");
            printf(" Stop program(0) --- Reset(5) --- Select MENU");
            
			
		    scanf("%d",&A);
		    switch(A) {
		    		case 1:    {	
						printf(" Find P\n\a");
                    	printf("Input V (m^3)\n :");
                    	scanf("%lf",&V);
                    	printf("Input n (mol) \n :");
                    	scanf("%lf",&n);
                    	printf("Input R (J/mol*K) \n :");
                    	scanf("%lf",&R);
                    	printf("Input T (K) \n :");
                    	scanf("%lf",&T);
                    	
                    	z=(n*R*T)/V;
                    	printf("value =%f N/m^2 \n\a",z);
                    	
						break;
                    	
	                 }
	                 case 2:    {	
						printf(" Find V\n\a");
                    	printf("Input P (N/m^2)\n :");
                    	scanf("%lf",&P);
                    	printf("Input n (mol)\n :");
                    	scanf("%lf",&n);
                    	printf("Input R (J/mol*K) \n :");
                    	scanf("%lf",&R);
                    	printf("Input T (K)\n :");
                    	scanf("%lf",&T);
                    	
                    	z=(n*R*T)/P;
                    	printf("value=%f (m^3)\n\a",z);
                    	
						break;
	}
				    case 3:   {	
						printf(" Find n\n\a");
                    	printf("Input P (N/m^2)\n :");
                    	scanf("%lf",&P);
                    	printf("Input V (m^3)\n :");
                    	scanf("%lf",&V);
                    	printf("Input R (J/mol*K)\n :");
                    	scanf("%lf",&R);
                    	printf("Input T (K)\n :");
                    	scanf("%lf",&T);
                    	
                    	z=(P*V)/(R/T);
                    	printf("value=%f\n\a",z);
                    	
						break;
	}
	                case 4:  {	
						printf(" Find T\n\a");
                    	printf("Input P \n :");
                    	scanf("%lf",&P);
                    	printf("Input V \n :");
                    	scanf("%lf",&V);
                    	printf("Input R \n :");
                    	scanf("%lf",&R);
                    	printf("Input n \n :");
                    	scanf("%lf",&n);
                    	
                        z=(P*V)/(n*R);
                    	printf("value=%f (mol)n\n\a",z);
                    	
						break;
                 
   }
	 	            case 5: {
					goto st;	
					break;
      				}        
					  default:
      			goto end;
    				}
						goto st;
		end:;

      
}


