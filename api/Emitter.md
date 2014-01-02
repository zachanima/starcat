# Emitter

Extends [Component].

## Description

Particle emitter attached to [GameObject].



## Variables

### duration

##### Number

Length of time emitter emits particles, in seconds. If looping, this indicates
one cycle.


### emission.bursts

##### Object

Particle bursts to emit over lifetime.

    // Emit 50 particles on start, and another 200 particles after 2.5 seconds.
    emitter.emission.bursts = { 0: 50, 2.5: 200 };


### emission.enabled

##### Boolean

Is particle emission enabled?


### emission.rate

##### Number

Particles per second to emit.


### gravityMultiplier

##### Number

Scales the gravity defined in [Physics].


### inheritVelocity

##### Boolean

Applies the current directional velocity of an attached Rigidbody, if any, to
newly emitted particles.


### looping

##### Boolean

If true, emission cycle will repeat after the duration.


### maxParticles

##### Number

Number of particles is limited by this number. Emission is temporarily halted if
this is reached.


### playOnAwake

##### Boolean

If true, emitter starts playing immediately.


### prewarm

##### Boolean

If true, particle emitter will have run for one cycle when starting.


### simulationSpace

##### [SimulationSpace]

In local space, particles stay relative to the emitter transform.


### startDelay

##### Number

Delay in seconds emitter will wait before emitting particles.


### startLifetime

##### Number

Start lifetime, in seconds. Particle is destroyed when lifetime reaches 0.


### startSpeed

##### Number

Start speed, in meters per second, applied in the starting direction.


### startSize

##### Number

Start size, in pixels.


### startRotation

##### Number

Start rotation, in radians.


### startColor

##### [Color]

Start color.


## Functions

### Emit

#### count

Emit `count` particles immediately.

    // Emit 100 particles immediately.
    emitter.Emit(100);



[Color]: #/Color
[Component]: #/Component
[GameObject]: #/GameObject
[Physics]: #/GameObject
[SimulationSpace]: #/SimulationSpace
