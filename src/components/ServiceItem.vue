<template>
    <div>
        <i :class="icon"></i>
        <hgroup>
            <h5>{{item}}</h5>
            <p>
                {{description}}
            </p>
        </hgroup>
    </div>
</template>

<script>
export default {
    name: 'ServiceItem',
    props:{
        item: String,
        description: String,
        icon: String
    }
}
</script>