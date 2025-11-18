Arduino code to read in controller inputs and output them over Arduino serial in a packet format to be parsed by the Godot project. Current reported values are:
{!lastStableButtonState,!currentSwitchState,lastForceSensor0Value,lastForceSensor1Value}
Button and switch state are inverted so that HIGH corresponds to the button/switch being on.
variable polling_rate_hz controls the rate at which values are reported by the controller. If set to <=0, this rate limit is ignored, and the controller instead reports values as soon as they are ready.
