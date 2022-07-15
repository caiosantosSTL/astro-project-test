<script>
    let clicked = false;
    function openList() {
        clicked = !clicked;
        if (clicked) {
            document.querySelector("#list-menu").classList.remove("sm:hidden");
            document.querySelector("#list-menu").classList.add("hidden");
        } else {
            document.querySelector("#list-menu").classList.remove("hidden");
            document.querySelector("#list-menu").classList.add("sm:hidden");
        }
    }
    let text = "";
</script>

<div>
    <nav
        id="nav"
        class="
        flex flex-row
        align-baseline
        justify-between
        p-4
        bg-gray-900
        text-white
      "
    >
        <div class="h-10 p-2">Logo</div>
        <div class="md:flex flex-row gap-2 hidden">
            <div class="h-10 p-2 bg- hover:bg-slate-500 cursor-pointer">
                Home
            </div>
            <div class="h-10 p-2 bg- hover:bg-slate-500 cursor-pointer">
                About
            </div>
        </div>
        <div
            id="list-menu-btn"
            class="
          md:hidden
          text-white
          h-10
          p-2
          flex
          align-baseline
          cursor-pointer
          bg-
          hover:bg-slate-500
        "
        >
            <div on:click={openList}>
                <p>menu-btn</p>
            </div>
        </div>
    </nav>
    <div
        id="list-menu"
        class="flex flex-col p-4 bg-gray-800 text-white md:hidden"
    >
        <div
            class="
          p-2
          h-10
          bg-
          hover:bg-slate-500
          flex
          justify-center
          cursor-pointer"
        >
            Menu
        </div>
        <div
            class="
          p-2
          h-10
          bg-
          hover:bg-slate-500
          flex
          justify-center
          cursor-pointer
        "
        >
            Menu
        </div>
    </div>
</div>
