<template>
  <transition name="modal">
    <div class="modal-mask">
      <div class="modal-wrapper">
        <div class="modal-container">
          <h3 slot="header">Диалог выбора элемента</h3>
          <div slot="body">
            <div class="filter-wrap">
              <div class="filter-wrap__item">
                <label for="search">Поиск</label>
                <input type="search" name="search">
              </div>
              <div class="filter-wrap_item filter-wrap__item_find">
                <label for="filter">Фильтр</label>
                <input type="search" name="filter">
              </div>
            </div>
            <div class="modal-find">
              <ul>
                <li>"element"</li>
              </ul>
            </div>
            <p>
              Выбранные элементы на данный момент:
            </p>
          </div>
        </div>
      </div>
    </div>
  </transition>
</template>


<script>

export default {
  name: 'Popup'
}
</script>

<style scoped>
    .modal-wrapper {
      width: 428px;
      background-color: rgba(0, 0, 0, 0.8);
      padding: 30px;
      color: #fff;
    }
    .modal-find {
      height: 280px;
      background-color: #000;
      overflow-y: auto;
      margin-top: 20px;
    }
    .modal-find li{
      display: block;
    }
    .filter-wrap {
      display: flex;
    }
    .filter-wrap__item_find {
      margin-left: 15px;
    }
    label {
      font-size: 14px;
      margin-right: 15px;
    }

    /* .modal-mask {
      position: fixed;
      z-index: 9998;
      top: 0;
      left: 0;
      width: 100%;
      height: 100%;
      background-color: rgba(0, 0, 0, .5);
      display: table;
      transition: opacity .3s ease;
    } */
</style>