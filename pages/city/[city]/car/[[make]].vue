<!-- Under pages u can create a folder that
creates subdomain/subpath under that u create
components that u can call and next release what pages
to call by folder stucture eg - under cars dir u create newcar component
it call when u hit url like - domain/city/newcar
-->
<!-- to make city name dynamic or can say call same path for
different cites like same for tornto and delhi 
wrap it under [] brackets, also work for both dir or component.
-->
<!-- U want to make it dynamic as well as optional 
wrap it against double nested [[]] brackets
-->
<!-- In this case we made a path under city dir which
creates a path to all pages we create under city
also we create a dynamic subdomain under that a static sub domain
car under that optional page/componet
which means 
if we call domain/city/delhi/car or domain/city/delhi/car/Tata 
in both cases this component is called by next.  
-->
<template>
    <div>
        <NavBar />
        <div class="mx-auto mt-4 max-w-7xl space-y-4 px-4 xs:px-8 sm:px-10 lg:px-16 pb-16 w-3/5">
            <div class="mt-32 flex">
                <CarSideBar />
                <CarCards />
            </div>
        </div>
    </div>
</template>