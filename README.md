# tmp

https://stackoverflow.com/questions/31541758/how-to-get-the-current-behave-step-with-python?rq=1

take a screenshot of a failed test, by setting an after_step hook in my environment.py file.
def after_step(context, step):
    if step.status == "failed":
        take_the_shot(context.scenario.name + " " + step.name)
        
def before_step(context, step):
    context.step = step


And the step implementation:
def step_impl(context):
    if some_condition:        
    


