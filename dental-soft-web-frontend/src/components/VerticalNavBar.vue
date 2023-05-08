<template>
    <v-card>
        <v-layout>
            <v-navigation-drawer permanent location="left">
                <template v-slot:prepend>
                    <v-list-item lines="two">
                        <div class="home-logo-wrapper">
                            <img src="../assets/logo.png" width="99" alt="logo" />
                            <h2 class="home-title">DentalSoft</h2>
                        </div>
                    </v-list-item>
                </template>
                <v-divider class="vertical-nav-divider"></v-divider>
                <v-list density="compact" nav>
                    <div class="mb-7 px-4">
                        <v-list-item prepend-icon="mdi-home-city" value="home">Overview</v-list-item>
                        <v-list-item prepend-icon="mdi-chart-line-variant" value="account">Booking Activity</v-list-item>
                        <v-list-item prepend-icon="mdi-wallet-bifold-outline" value="users">Wallet</v-list-item>
                        <v-list-item prepend-icon="mdi-cog" value="users">Settings</v-list-item>
                    </div>
                    <v-divider class="vertical-nav-divider"></v-divider>
                    <div class="mt-6 px-4">
                        <v-list-item prepend-icon="mdi-email" value="users">Inbox</v-list-item>
                        <v-list-item prepend-icon="mdi-bell" value="users">Notifications</v-list-item>
                        <v-list-item prepend-icon="mdi-badge-account" value="users">Support</v-list-item>
                    </div>
                </v-list>
            </v-navigation-drawer>
            <v-main style="height: 250px"></v-main>
        </v-layout>
    </v-card>
</template>

<script>
export default {
    data() {
        return {
            items: [
                { title: 'Home', icon: 'mdi-home-city' },
                { title: 'My Account', icon: 'mdi-account' },
                { title: 'Users', icon: 'mdi-account-group-outline' },
            ],
        }
    },
}
</script>

<style>
.home-logo-wrapper {
    display: flex;
    align-items: center;
}

.vertical-nav-divider {
    margin-left: 1rem;
    margin-right: 1rem;
}
</style>