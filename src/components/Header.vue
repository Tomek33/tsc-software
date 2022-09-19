<template>
    <div>
        <nav class="navbar navbar-expand-sm">
            <div class="container-fluid">
                <a class="navbar-brand" href="#">
                    <div class="d-flex align-items-center">
                        <img src="../assets/nav-image.png" alt="Bootstrap" width="30" height="24">
                        <span class="my-text-header ms-2">Start</span>
                    </div>
                </a>
                <button class="navbar-toggler" type="button" data-bs-toggle="collapse" data-bs-target="#navbarNav" aria-controls="navbarNav" aria-expanded="false" aria-label="Toggle navigation">
                <span class="navbar-toggler-icon"></span>
                </button>
                <div class="collapse navbar-collapse justify-content-end" id="navbarNav">
                <ul class="navbar-nav">
                    <li class="nav-item">
                        <a class="nav-link" href="#">
                            <span class="my-text-link">
                                Home
                            </span>
                        </a>
                    </li>
                    <li class="nav-item">
                        <a class="nav-link" href="#">
                            <span class="my-text-link">
                                Portfolio
                            </span>
                        </a>
                    </li>
                    <li class="nav-item">
                        <a class="nav-link" href="#">
                            <span class="my-text-link">
                                Services
                            </span>
                        </a>
                    </li>
                    <li class="nav-item">
                        <a class="nav-link" href="#">
                            <span class="my-text-link">
                                Contact
                            </span>
                        </a>
                    </li>
                </ul>
                </div>
            </div>
        </nav>
    </div>
</template>

<style scoped>
    .my-text-header{
        color: #FFFFFF;
        font-family: 'Work Sans';
        font-size: 40px;
    }

    .my-text-link{
        color: #FFFFFF;
        font-family: 'Roboto';
        font-size: 16px;
    }
</style>

<script>
    export default {
    name: "Header"
}
</script>