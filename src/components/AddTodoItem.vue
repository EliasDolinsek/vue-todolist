<template>
    <div class="card">
        <div class="card-header">
            Add Todo Item
        </div>
        <div class="card-body">
            <form @submit.prevent="submit">
                <div class="form-group">
                    <label for="title">Title</label>
                    <input v-model="title" type="text" class="form-control" id="title" aria-describedby="titleHelp"
                        placeholder="Title">
                    <small id="titleHelp" class="form-text text-muted">What do you want to do?</small>
                </div>
                <div class="form-group">
                    <label for="deadline">Date</label>
                    <input v-model="deadline" type="date" class="form-control" id="deadline" placeholder="Deadline">
                </div>
                <button type="submit" class="btn btn-primary mt-3">Add item</button>
            </form>
        </div>
    </div>
</template>
<script>
export default {
    name: "AddTodoItem",
    data() {
        return {
            title: "",
            deadline: "2022-06-02"
        }
    },
    methods: {
        submit(){
            console.log(name)
        }
    }
}
</script>