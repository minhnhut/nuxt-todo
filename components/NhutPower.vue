<template>
    <div>
        <input type="text" v-model="currentInput">
        <button @click.prevent="add()">Add</button>
        <ul>
            <li :key="key" v-for="(todo, key) in todos">
                {{todo}} - {{key}}
            </li>
        </ul>
    </div>
</template>

<script>
export default {
    data: () => ({
        todos: [],
        currentInput: ""
    }),
    methods: {
        add() {
            this.todos.push(this.currentInput);
            this.currentInput = "";
        },
    }
};
</script>
