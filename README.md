# calculator-using-oops

#BLL

#class
class Calculator:
    def __init__(self):
        self.x = 0
        self.y = 0
        self.z = 0

    #function for ADD

    def add(self):
        self.z = self.x + self.y
        return self.z

    #function for subtract

    def sub(self):
        self.z = self.x - self.y
        return self.z

    #function for multiply

    def mul(self):
        self.z = self.x * self.y
        return self.z

    #function for divide

    def div(self):
        self.z = self.x / self.y
        return self.z



#PL

#infinite loop
while True:
    print('WELCOME TO MY CALCULATOR')
    print('1. ADD \n 2. SUBTRACT \n 3. MULTIPLY \n 4. DIVIDE')

    choice = input('enter your choice: ')  # take choice from user

    ob = Calculator() #we need to access the class so we create a class as a object

    ob.x = int(input('enter the first number: '))
    ob.y = int(input('enter the second number: '))

    if choice == '1': #if user choose 1 for ADD
        ob.add()
        print('the sum of',ob.x, 'and', ob.y,'is: ', ob.z)

    elif choice == '2': #if user choose 2 for SUB
        ob.sub()
        print('the sub of',ob.x, 'and', ob.y,'is: ', ob.z)

    elif choice == '3': #if user choose 3 for mul
        ob.mul()
        print('the mul of',ob.x, 'and', ob.y,'is: ', ob.z)

    elif choice == '4': #if user choose 4 for div
        ob.div()
        print('the div of',ob.x, 'and', ob.y,'is: ', ob.z)
