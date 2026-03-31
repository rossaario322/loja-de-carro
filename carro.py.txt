class Vehicle:
    color = "white"

    def __init__(self, max_speed, mileage):
        self.max_speed = max_speed
        self.mileage = mileage
        self.seating_capacity = None

    def assign_seating_capacity(self, seating_capacity):
        self.seating_capacity = seating_capacity

    def display_properties(self):
        print("Properties of the Vehicle:")
        print("Color:", self.color)
        print("Maximum Speed:", self.max_speed)
        print("Mileage:", self.mileage)
        print("Seating Capacity:", self.seating_capacity)

carro1 = Vehicle(200, 20)
carro1.assign_seating_capacity(5)

carro2 = Vehicle(180, 25)
carro2.assign_seating_capacity(4)


numero = int(input("qual carro você quer? o 1 ou o 2?"))

if numero == 1:
   carro1.display_properties()
elif numero == 2:
    carro2.display_properties()

else:
    print("Escolha inválida")

