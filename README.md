# SKT
初级Java取余运算，简单逻辑设计
package com.java.javaBool;

public class daa {
	
	private int add(int x,int t)
	{
	    int zub=t;//被除数
	    int zud=-1;//余数
	    if(t==0)
	    	return -1;
		if(x<t)                              //除数小于被除数直接被除数就是余数
			return x; 
		else
		{                                    //除数大于等于被除数时，余数就是除数减去被除数乘最大至小于t
			for	(int i=1;zub>=t;i++)
			{
				zub=x-i*t;
			}
			zud=zub;
			return zud;
		}
	}
	

	public static void main(String[] args) {
		// TODO Auto-generated method stu
		int a=5555,b=16;
		System.out.println(new daa().add(a,b));
        System.out.println(a%b);
	}

