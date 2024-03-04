<!-- layout is to create one single pattern/Design for more than one place -->
<!-- dir should be named layouts -->
<!-- this file is specifically named default because this is the default design we want -->

<template>
    <div>
        <NavBar />
            <!-- It's a vue 3 component act as a placeholder to render all other html we wrote in compnents -->
        <slot />
    </div>
</template>