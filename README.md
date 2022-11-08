# example-customHook-forhttpRequest

#### the idea is using custom Hooks for http request, reusing code, passing by parameters data transformations and the data for the request. I use a firebase DB for playing.

##### 
the function MUST start with “use”.. 
so if you create an state in your customized hook , that state will be tied to those components which will be call that hook. 
every component will be received its own states. shares the logic not the concrete state. 

so when you pass parameters to a customized hook, and there are objects or functions( they are objects as well).. 
those parameters could change in the component the pointer will be change every in evert component rendering, 
so two approaches or you use usecallbacks in the functions that you want to pass to the customized hook, 
or you return the function that you wrapped up in the customized hook and use that function with the parameters from the component without 
tied the objects to a rerender. 
