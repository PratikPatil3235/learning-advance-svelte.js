<div class="card">
  <div class="card-header">
    <slot name="header"></slot>
  </div>
  <div class="card-content">
    <slot name="content">Default Content</slot>
  </div>
  {#if $$slots.footer}
  <hr>
  <div class="card-footer">
    <slot name="footer"></slot>
  </div>
  {/if}
</div>

<style>
  .card {
    box-shadow: 0 4px 8px 0 rgba(0, 0, 0, 0.2);
    transition: 0.3;
    padding: 16px;
    margin-bottom: 20px;
    width: 100%;
  }
  .card:hover {
    box-shadow: 0 8px 16px 0 rgba(0, 0, 0, 0.2);
  }
</style>
