# Data Oriented Design

- Organizing data for efficient processing 
- Reducing cache misses

Note:
aka. Data Oriented Programming

--

```C
class Ball {
    Point  position;
    Color  color;
    double radius;
    void draw();
};

vector<Ball> balls; // classical OOP

class Balls { 
    vector<Point>  position; // DOD:
    vector<Color>  color;    // arrays of properties
    vector<double> radius;   // NOT arrays of objects
    void draw();
};
```

--

# Entity Component System

- Composition over inheritance principle
- **ENTITY** - general purpose object, usually has ID
- **COMPONENT** - labels the Entity as possessing a particular aspect
- **SYSTEM** - performs actions on every Entity which posesses a specific Component

Note:
Entity = game objects  
Components = physics, gravity, acceleration, drawable
