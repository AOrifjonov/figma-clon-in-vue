<script>
export default {
    data() {
        return {
            cards: true,
            lists: false
        }
    },

    methods: {
        activeCards() {
            this.cards = true
            this.lists = false
        },
        activeLists() {
            this.lists = true
            this.cards = false
        }
    }
}
</script>

<template>
    <div class="top"></div>
    <div class="elements">
        <div class="element">
            <div class="card">
                <span class="opt">Filter: </span> All files
                <div style="display: flex; justify-content: end; align-items: center;">
                    <span class="opt">Sort:  </span> Last viewed 
                    <button @click="activeCards" :class="cards ? `btn active` : 'btn'">
                        <svg class="svg" width="12" height="12" viewBox="0 0 12 12" xmlns="http://www.w3.org/2000/svg"><path d="M1 1h3v3H1V1zM0 0h5v5H0V0zm1 8h3v3H1V8zM0 7h5v5H0V7zm11-6H8v3h3V1zM8 0H7v5h5V0H8zm0 8h3v3H8V8zM7 7h5v5H7V7z" fill-rule="evenodd" fill-opacity="1" fill="#000" stroke="none"></path></svg>
                    </button>
                    <button @click="activeLists" :class="lists ? `btn active` : 'btn'">
                        <svg class="svg" width="14" height="11" viewBox="0 0 14 11" xmlns="http://www.w3.org/2000/svg"><path d="M0 0h14v1H0V0zm0 5h14v1H0V5zm14 5H0v1h14v-1z" fill-rule="evenodd" fill-opacity=".8" fill="#000" stroke="none"></path></svg>
                    </button>
                </div>
            </div>
            <div v-if="cards" class="cards">
                <div class="item">
                    <div class="photo">
                        <img src="@/assets/card-1.png" alt="Photo 1">
                    </div>
                    <div class="body">
                        <svg class="svg" width="32" height="32" viewBox="0 0 32 32" xmlns="http://www.w3.org/2000/svg"><path d="M7 28h18c.552 0 1-.448 1-1V9.914c0-.265-.105-.52-.293-.707l-4.914-4.914C20.605 4.105 20.35 4 20.086 4H7c-.552 0-1 .448-1 1v22c0 .552.448 1 1 1z" fill-rule="nonzero" fill-opacity="1" fill="#9747ff" stroke="none"></path><path d="M19.297 20.862c.184.184.483.184.668 0l1.04-1.041c.185-.185.185-.484 0-.669l-5.947-5.948-1.71 1.71 5.949 5.948zm-6.655-6.655l-.94-.94-.427-2.136 2.136.427.94.94-1.71 1.709zm-1.58-4.139l2.842.569 7.809 7.808c.575.575.575 1.508 0 2.083l-1.041 1.04c-.575.576-1.508.576-2.082 0l-7.81-7.808-.567-2.842L10 9.856l1.062.212z" fill-rule="evenodd" fill-opacity="1" fill="#fff" stroke="none"></path><path d="M20.5 8.5V4l1.707 1.707 2.086 2.086L26 9.5h-4.5c-.552 0-1-.448-1-1z" fill-rule="nonzero" fill-opacity="1" fill="#c599ff" stroke="none"></path></svg>
                        <div>
                            FigJam Basics
                            <p>In drafts - Edited 19 days ago</p>
                        </div>
                    </div>
                </div>

                <div class="item">
                    <div class="photo">
                        <img src="@/assets/card-2.png" alt="Photo 1">
                    </div>
                    <div class="body">
                        <svg class="svg" width="32" height="32" viewBox="0 0 32 32" xmlns="http://www.w3.org/2000/svg"><path d="M7 28h18c.552 0 1-.448 1-1V9.914c0-.265-.105-.52-.293-.707l-4.914-4.914C20.605 4.105 20.35 4 20.086 4H7c-.552 0-1 .448-1 1v22c0 .552.448 1 1 1z" fill-rule="nonzero" fill-opacity="1" fill="#18a0fb" stroke="none"></path><path d="M16.858 12.995l-.011-.003-4.403-1.255 3.257 3.257c.116-.04.24-.062.37-.062.628 0 1.138.51 1.138 1.139 0 .628-.51 1.138-1.138 1.138-.629 0-1.139-.51-1.139-1.138 0-.13.022-.254.062-.37l-3.252-3.251 1.202 4.192.01.036.008.038c.298 1.443 1.578 2.528 3.109 2.528.349 0 .683-.056.995-.159l.585-.193.435.436 1.231 1.23 1.269-1.268-1.245-1.244-.43-.431.184-.58c.097-.303.15-.627.15-.964 0-1.476-1.009-2.719-2.375-3.073l-.012-.003zm4.435 5.588l.707.707-.707.707-1.269 1.269-.707.707-.707-.707-1.23-1.231c-.412.136-.852.21-1.31.21-2.014 0-3.696-1.428-4.087-3.328l-1.658-5.785L10 10l1.133.323 5.988 1.707c1.797.466 3.123 2.098 3.123 4.04 0 .443-.068.869-.196 1.268l1.245 1.245z" fill-rule="evenodd" fill-opacity="1" fill="#fff" stroke="none"></path><path d="M20.5 8.5V4l1.707 1.707 2.086 2.086L26 9.5h-4.5c-.552 0-1-.448-1-1z" fill-rule="nonzero" fill-opacity="1" fill="#9bd5fd" stroke="none"></path></svg>
                        <div>
                            Figma basics
                            <p>In drafts - Edited 19 days ago</p>
                        </div>
                    </div>
                </div>

                <div class="item">
                    <div class="photo">
                        <img src="@/assets/card-3.png" alt="Photo 1">
                    </div>
                    <div class="body">
                        <svg class="svg" width="32" height="32" viewBox="0 0 32 32" xmlns="http://www.w3.org/2000/svg"><path d="M7 28h18c.552 0 1-.448 1-1V9.914c0-.265-.105-.52-.293-.707l-4.914-4.914C20.605 4.105 20.35 4 20.086 4H7c-.552 0-1 .448-1 1v22c0 .552.448 1 1 1z" fill-rule="nonzero" fill-opacity="1" fill="#18a0fb" stroke="none"></path><path d="M16.858 12.995l-.011-.003-4.403-1.255 3.257 3.257c.116-.04.24-.062.37-.062.628 0 1.138.51 1.138 1.139 0 .628-.51 1.138-1.138 1.138-.629 0-1.139-.51-1.139-1.138 0-.13.022-.254.062-.37l-3.252-3.251 1.202 4.192.01.036.008.038c.298 1.443 1.578 2.528 3.109 2.528.349 0 .683-.056.995-.159l.585-.193.435.436 1.231 1.23 1.269-1.268-1.245-1.244-.43-.431.184-.58c.097-.303.15-.627.15-.964 0-1.476-1.009-2.719-2.375-3.073l-.012-.003zm4.435 5.588l.707.707-.707.707-1.269 1.269-.707.707-.707-.707-1.23-1.231c-.412.136-.852.21-1.31.21-2.014 0-3.696-1.428-4.087-3.328l-1.658-5.785L10 10l1.133.323 5.988 1.707c1.797.466 3.123 2.098 3.123 4.04 0 .443-.068.869-.196 1.268l1.245 1.245z" fill-rule="evenodd" fill-opacity="1" fill="#fff" stroke="none"></path><path d="M20.5 8.5V4l1.707 1.707 2.086 2.086L26 9.5h-4.5c-.552 0-1-.448-1-1z" fill-rule="nonzero" fill-opacity="1" fill="#9bd5fd" stroke="none"></path></svg>
                        <div>
                            Prototyping in figma
                            <p>In drafts - Edited 19 days ago</p>
                        </div>
                    </div>
                </div>
            </div>
            <div v-if="cards" class="cards">
                <div class="item">
                    <div class="photo">
                        <img src="@/assets/card-4.png" alt="Photo 1">
                    </div>
                    <div class="body">
                        <svg class="svg" width="32" height="32" viewBox="0 0 32 32" xmlns="http://www.w3.org/2000/svg"><path d="M7 28h18c.552 0 1-.448 1-1V9.914c0-.265-.105-.52-.293-.707l-4.914-4.914C20.605 4.105 20.35 4 20.086 4H7c-.552 0-1 .448-1 1v22c0 .552.448 1 1 1z" fill-rule="nonzero" fill-opacity="1" fill="#18a0fb" stroke="none"></path><path d="M16.858 12.995l-.011-.003-4.403-1.255 3.257 3.257c.116-.04.24-.062.37-.062.628 0 1.138.51 1.138 1.139 0 .628-.51 1.138-1.138 1.138-.629 0-1.139-.51-1.139-1.138 0-.13.022-.254.062-.37l-3.252-3.251 1.202 4.192.01.036.008.038c.298 1.443 1.578 2.528 3.109 2.528.349 0 .683-.056.995-.159l.585-.193.435.436 1.231 1.23 1.269-1.268-1.245-1.244-.43-.431.184-.58c.097-.303.15-.627.15-.964 0-1.476-1.009-2.719-2.375-3.073l-.012-.003zm4.435 5.588l.707.707-.707.707-1.269 1.269-.707.707-.707-.707-1.23-1.231c-.412.136-.852.21-1.31.21-2.014 0-3.696-1.428-4.087-3.328l-1.658-5.785L10 10l1.133.323 5.988 1.707c1.797.466 3.123 2.098 3.123 4.04 0 .443-.068.869-.196 1.268l1.245 1.245z" fill-rule="evenodd" fill-opacity="1" fill="#fff" stroke="none"></path><path d="M20.5 8.5V4l1.707 1.707 2.086 2.086L26 9.5h-4.5c-.552 0-1-.448-1-1z" fill-rule="nonzero" fill-opacity="1" fill="#9bd5fd" stroke="none"></path></svg>
                        <div>
                            Wireframing in Figma
                            <p>In drafts - Edited 19 days ago</p>
                        </div>
                    </div>
                </div>
            </div>

            <div v-if="lists" class="lists">
                <div class="lists">
                    <div class="sort">
                        <div class="sort2">
                            File name
                        </div>
                        <div class="sort2">
                            Last viewed
                        </div>
                    </div>

                    <div class="listItem">
                        <div class="list">
                            <img src="@/assets/card-1.png" alt="">
                            FigJam basics
                        </div>
                        <div class="list">
                            19 days ago
                        </div>
                    </div>

                    <div class="listItem">
                        <div class="list">
                            <img src="@/assets/card-2.png" alt="">
                            Figma basics
                        </div>
                        <div class="list">
                            19 days ago
                        </div>
                    </div>

                    <div class="listItem">
                        <div class="list">
                            <img src="@/assets/card-3.png" alt="">
                            Prototyping in Figma
                        </div>
                        <div class="list">
                            19 days ago
                        </div>
                    </div>

                    <div class="listItem">
                        <div class="list">
                            <img src="@/assets/card-4.png" alt="">
                            Wireframing in figma
                        </div>
                        <div class="list">
                            19 days ago
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </div>
</template>

<style scoped>
    /* Cards */
    .top {
        height: 236px;
    }
    .elements {
        margin-left: 236px;
    }

    .element {
        padding: 10px;
    }

    .card {
        font-size: 12px;
    }
    span {
        color: #acacac;
    }
    button {
        display: flex;
        align-items: center;
        margin: 0 7px;
        outline: none;
        background: none;
        border: 1px solid #dadada;
        border-radius: 4px;
        padding: 6px;
    }
    .cards {
        display: flex;
        width: 100%;
        justify-content: flex-start;
        padding: 20px;
    }
    .item {
        width: 333px;
        height: 300px;
        background: #fff;
        border: 2px solid #dadada;
        border-radius: 10px;
        margin: 0 15px;
    }
    .item .photo {
        display: flex;
        height: 220px;
        width: 330px;
        background: #dadada;
        align-items: center;
    }
    .item .photo img {
        width: 100%;
    }
    .body {
        display: flex;
        height: 80px;
        align-items: center;
        font-size: 14px;
        color: #444343;
    }
    .body svg {
        margin-right: 10px;
    }
    .body div p {
        font-size: 12px;
        padding-top: 2px;
        color: #acacac;
    }
    .opt {
        margin-right: 10px;
    }
    .active {
        border: 1px solid blue;
        color: blue;
    }


    /* List */
    .lists {
        padding: 15px;
    }
    .list {
        display: flex;
        align-items: center;
        width: 100%;
        margin: 5px 0;
        font-size: 13px;

    }
    .list img {
        width: 25px;
        height: 25px;
        margin-right: 15px;
    }
    .sort {
        display: flex;
        margin-bottom: 20px;
        font-size: 12px;
    }
    .sort2 {
        display: flex;
        width: 50%;
        justify-content: flex-start;
        color: #c0c0c0;
        font-size: 13px;
    }
    .listItem {
        display: flex;
        align-items: center;
        margin: 5px 0;
    }
</style>