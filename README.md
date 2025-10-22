# object-oriented-programming
this program shows how polymorphism works
[object oriented programming.py](https://github.com/user-attachments/files/23050488/object.oriented.programming.py)
# vehicles.py

# Base class
class Vehicle:
    def move(self):
        raise NotImplementedError("Subclasses must implement this method")

# Subclasses
class Car(Vehicle):
    def move(self):
        print("🚗 The car is driving on the road.")

class Plane(Vehicle):
    def move(self):
        print("✈️ The plane is flying in the sky.")

class Boat(Vehicle):
    def move(self):
        print("🚤 The boat is sailing on the water.")

class Bicycle(Vehicle):
    def move(self):
        print("🚴 The bicycle is pedaling along the path.")

# Demonstration of polymorphism
def show_movement(vehicles):
    for v in vehicles:
        v.move()

# Create a list of different vehicle objects
vehicles = [Car(), Plane(), Boat(), Bicycle()]

# Show how each moves differently
show_movement(vehicles)
