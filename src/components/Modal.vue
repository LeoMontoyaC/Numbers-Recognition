<template>
    <div class="modal">
      <div class="modal-container">
        <button class="modal-close">X</button>
        <p class="answer-keras text-dark"></p>
        <div class="flex-center">
          <div class="spinner"></div>
        </div>
        <img
          src="{{ url_for('static', filename='assets/cheque.svg') }}"
          width="120"
          height="120"
          alt=""
        />
      </div>
    </div>
</template>

<style>
  .modal {
  position: fixed;
  z-index: 1000;
  top: 0;
  left: 0;
  width: 100%;
  min-height: 100vh;
  background-color: var(--opacity-color);
  display: none;
  justify-content: center;
  align-items: center;
}

.modal.is-open {
  display: flex;
}

.modal-container {
  position: relative;
  padding: 1rem;
  width: 24vw;
  height: 20vw;
  min-width: 300px;
  min-height: 240px;
  max-width: 840px;
  max-height: 780px;
  overflow-y: auto;
  border-radius: 8px;
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;
  background-color: var(--white-color-h);
}

.modal-close {
  position: absolute;
  cursor: pointer;
  top: 1rem;
  right: 1rem;
  font-weight: bold;
  font-size: 16px;
  color: var(--border-color);
  border-radius: 4px;
  width: 2rem;
  height: 2rem;
  background-color: rgba(218, 62, 62, 0.9);
  border-style: none;
}

.text-dark {
  color: var(--dark-color);
  line-height: 2.4rem;
  text-align: center;
  letter-spacing: 2px;
  font-size: calc(1.275vw + 1.725vh);
}

/*Spinner de carga*/

.flex-center {
  display: none;
  justify-content: center;
  align-items: center;
}

.spinner {
  border: 14px solid rgba(0, 0, 0, 0.2);
  width: 124px;
  height: 124px;
  border-radius: 50%;
  border-left-color: #09f;

  animation: spin 2s ease infinite;
}

@keyframes spin {
  0% {
    transform: rotate(0deg);
  }

  100% {
    transform: rotate(360deg);
  }
}

@media (max-width: 960px) {
  .credits__flaticon {
    display: none !important;
  }

  .credits__user {
    grid-column: 1 / 3;
  }

  .btn__clear {
    justify-content: center;
    padding: 0;
    margin: 0;
  }

  .btn__clear p {
    font-size: 1.4rem;
  }

  .btn__clear img {
    display: none !important;
  }
}
</style>