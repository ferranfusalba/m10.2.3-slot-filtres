<template>
  <div>
    <div class="modal" id="modalCurrency" tabindex="-1" role="dialog" aria-labelledby="modalCurrencyLabel" aria-hidden="true">
      <div class="modal-dialog" role="document">
        <div class="modal-content">

          <div class="modal-header">
            <slot name="header"></slot>
          </div>

          <div class="modal-body">
            <slot name="body"></slot>
            <p>
              <br>
            El canvi de {{ euros }} € a dòlars són {{ euros | euroDolar }} $
            </p>
          </div>

          <div class="modal-footer">
            <slot name="footer"></slot>
          </div>
          
        </div>
      </div>
    </div>
  </div>
</template>

<script src="../scripts/ModalBootstrap.js"></script>