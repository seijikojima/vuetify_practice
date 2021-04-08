<template>
    <v-container>
    <nav>
        <v-toolbar flat app>  
            <v-app-bar-nav-icon @click="drawer=!drawer"></v-app-bar-nav-icon>


            <v-toolbar-title class="text-uppercase grey--text">
                <span class="font-weight-light">Todo</span>
                <span>Sabosan</span>
            </v-toolbar-title>

            <v-spacer></v-spacer>
            <v-btn flat color="gery">
            <span>SIGN OUT</span>
            <v-icon right>exit_to_app</v-icon>
            </v-btn>

        </v-toolbar>

        <v-navigation-drawer app v-model="drawer" class="primary">
            <v-list>
           
                <v-list-item v-for="link in links" :key="link.text" :href="link.route">
                    
                    <v-list-content>
                        <v-list-item-icon>
                            <v-icon class="white--text" v-text="link.icon"></v-icon>
                        </v-list-item-icon>
                    </v-list-content>

                    <v-list-item-content>                 
                        <v-list-title class="white--text" v-text="link.text"></v-list-title>
                    </v-list-item-content>

                </v-list-item>
                
            </v-list>
        </v-navigation-drawer>

    </nav>
    </v-container>
</template>

<script>

export default ({

    data() {
        return {
            drawer : false,
            links: [
                { icon: "dashboard", text:"Dashboard", route: '/'},
                { icon: "folder", text:"Projects", route: '/projecsts'},
                { icon: "person", text:"Team", route: '/team'},
            ]
        }
    }

})
</script>
