<style>
    :global(h1, .h1, h2, .h2, h3, .h3, h4, .h4, h5, .h5, h6, .h6) {
        color: #222;
        font-family: lato,sans-serif;
        font-weight: 700;
        line-height: 1.2;
    }

    :global(h4, .h4) {
        font-size: 20px;
    }

    :global(.section) {
        padding-top: 70px;
        padding-bottom: 70px;
    }

    :global(.bg-light) {
        background-color: #edf6f5!important;
    }

    :global(p, .paragraph) {
        font-weight: 400;
        color: #777;
        font-size: 16px;
        line-height: 1.7;
        font-family: lato,sans-serif;
    }

    :global(.btn-primary) {
    /*background-color: royalblue;*/
        background-color: #0aa8a7;
        color: #fff;
        border-color: #0aa8a7;
    }

    :global(.btn-sm) {
        padding: 12px 30px;
        font-size: 15px;
    }

    :global(.btn) {
        font-size: 16px;
        font-family: lato,sans-serif;
        font-weight: 600;
        text-transform: capitalize;
        padding: 15px 30px;
        border-radius: 30px;
        border: 0;
        border-top-color: currentcolor;
        border-right-color: currentcolor;
        border-bottom-color: currentcolor;
        border-left-color: currentcolor;
        position: relative;
        z-index: 1;
        transition: .2s ease;
        white-space: nowrap;
    }

    :global(.btn::before) {
        position: absolute;
        content: "";
        height: 100%;
        width: 100%;
        top: 50%;
        left: 50%;
        transform: translate(-50%,-50%);
        z-index: -1;
        border-radius: inherit;
        transition: inherit;
        background-color: inherit;
        border: 1px solid transparent;
    }

    :global(.btn:hover::before, .btn:active::before, .btn:focus::before) {
        height: 110%;
        width: 110%;
    }

  :global(.btn-primary:active, .btn-primary:hover, .btn-primary.focus, .btn-primary.active) {
    background-color: #0aa8a7 !important;
        border-color: #0aa8a7 !important;
    }
</style>
