<template>
    <ul class="main-menu nav">
        <li>
            <n-link to="/">Home</n-link>
        </li>
        <li>
            <n-link to="/about">About Us</n-link>
        </li>
        <li class="has-submenu">
            <n-link to="/causes">Causes</n-link>
            <ul class="submenu-nav">
                <li>
                    <n-link to="/causes">Causes</n-link>
                </li>
                <li>
                    <n-link to="/causes-details">Causes Details</n-link>
                </li>
            </ul>
        </li>
        <li class="has-submenu">
            <n-link to="/blog">Blog</n-link>
            <ul class="submenu-nav">
                <li>
                    <n-link to="/blog">Blog</n-link>
                </li>
                <li>
                    <n-link to="/blog-details">Blog Details</n-link>
                </li>
            </ul>
        </li>
        <li class="has-submenu">
            <n-link to="/event-details">Pages</n-link>
            <ul class="submenu-nav">
                <li>
                    <n-link to="/event-details">Event Details</n-link>
                </li>
                <li>
                    <n-link to="/volunteer">Volunteer</n-link>
                </li>
                <li>
                    <n-link to="/donation">Donation</n-link>
                </li>
            </ul>
        </li>
        <li>
            <n-link to="/contact">Contact Us</n-link>
        </li>
    </ul>
</template>