```mermaid
classDiagram
    class Animal {
        +String name
        +String birthDate
        +List~String~ commands
        +addCommand(String command)
        +listCommands() List~String~
    }

    class PetAnimal {
        +String breed
    }

    class PackAnimal {
        +float maxLoad
    }

    class Dog {
        +bark() String
    }

    class Cat {
        +meow() String
    }

    class Hamster {
        +run() String
    }

    class Horse {
        +gallop() String
    }

    class Camel {
        +store_water() String
    }

    class Donkey {
        +carry() String
    }

    Animal <|-- PetAnimal
    Animal <|-- PackAnimal
    PetAnimal <|-- Dog
    PetAnimal <|-- Cat
    PetAnimal <|-- Hamster
    PackAnimal <|-- Horse
    PackAnimal <|-- Camel
    PackAnimal <|-- Donkey