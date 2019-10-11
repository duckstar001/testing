 New tutorial not using extension

# Motion with the Microbit

## Introduction @unplugged
Make things move using a servo. Boo!

## Step 1

Today we are going to make things move using the Microbit. 
We are going to connect a servo.

## Step 3

Add two ``||pins:servo write pin||`` blocks to the ``||basic:forever||`` block.  
One should be set to 0 degrees and the other set to 180 degrees.  
The blocks are the below the black Advanced tab. 

```blocks
basic.forever(function () {
    pins.servoWritePin(AnalogPin.P0, 0)
})
```

## Step 4

Add two  ``||basic:pause||`` blocks to the ``||basic:forever||`` block.

```blocks
basic.forever(function () {
    basic.pause(1000)
})
```

## Step 5

Your code should now look like this.

```blocks
basic.forever(function () {
    pins.servoWritePin(AnalogPin.P0, 0)
    basic.pause(1000)
    pins.servoWritePin(AnalogPin.P0, 180)
    basic.pause(1000)
})
```

## Step 6 @unplugged

Now tweak your code to get your servo moving how you would like. 

