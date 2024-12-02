<template>
    <Link
        class="text-blue-500 hover:underline"
        :class="{ 'font-bold underline': active }"
    >
        <slot />
    </Link>
</template>

<script>
import { Link } from "@inertiajs/vue3";

export default {
    // eslint-disable-next-line vue/no-reserved-component-names
    components: { Link },
    props: {
        active: Boolean,
    },
};
</script>
