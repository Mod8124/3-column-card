<template>
    <div class="card" :class="{first: theme === 'first', second: theme === 'second', third: theme === 'third'}">
            <div class="img">
               <slot name="img"></slot>
            </div>

            <div class="tittle">
                 <h3>
                     <slot name="title"></slot>
                </h3>
            </div>


            <div class="text">
                <p>
                    <slot name="text"></slot>
                </p>
            </div>

        <div class="button">
            <button :class="{colorFirst: theme === 'first', colorSecond : theme === 'second', colorThird : theme === 'third'}">Learn More</button>
        </div>
    </div>
</template>

<script>
export default {
    props:['theme'],
}
</script>