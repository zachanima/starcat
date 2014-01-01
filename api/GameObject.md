# GameObject

## Description

Entity in [Scene].



## Constructors

### GameObject

#### [name], [componentClass, ...]

Creates game object named `name`, and attaches new components of the types
of `componentClass` arguments.

    // Create game object named 'Player', and attach Emitter and Rigidbody.
    new GameObject('Player', Emitter, Rigidbody);



## Variables

### gameObject

##### GameObject

This game object.


### transform

##### [Transform]

The transform attached to this game object.



## Functions

### AddComponent

#### componentClass

##### [Component]

Attaches new component of type `componentClass` to this game object. The
attached component is returned.

    // Attach Rigidbody component to game object.
    gameObject.AddComponent(Rigidbody);


### GetComponent

#### componentClass

##### [Component]

Returns first component of type `componentClass` attached to this game object.

    // Retrieve custom `Foo.Bar` component attached to game object.
    var baz = gameObject.GetComponent(Foo.Bar);


### SendMessage

#### methodName, value

Calls method named `methodName`, with argument `value` on every component
attached to this game object.

    // Call method `Damage` with argument `50` on every attached component.
    gameObject.SendMessage('Damage', 50);


[Component]: #/Component
[Scene]: #/Scene
[Transform]: #/Transform
