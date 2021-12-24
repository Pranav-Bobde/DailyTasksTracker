<template>
  <q-list
    class="rounded-borders"
    bordered
    separator
  >
      <q-item-label>
          <q-item>
            <q-item-section class="col-1">
              <q-item-label class="text-h6 text-center">
                Sr.
              </q-item-label>
            </q-item-section>

            <q-item-section class="col-2">
              <q-item-label class="text-h6 text-center">
                Title
              </q-item-label>
            </q-item-section>

            <q-item-section>
              <q-item-label class="text-h6 text-center">
                Remaining
              </q-item-label>
            </q-item-section>

            <q-item-section>
              <q-item-label class="text-h6 text-center">
                Total
              </q-item-label>
            </q-item-section>

            <q-item-section>
              <q-item-label class="text-h6 text-center">
                Rate(per day)
              </q-item-label>
            </q-item-section>

            <q-item-section>
              <q-item-label class="text-h6 text-center">
                Days Remaining
              </q-item-label>
            </q-item-section>
          </q-item>
      </q-item-label>

      <q-item v-for="item in items" :key="item.index">
        <q-item-section class="col-1">
          <q-item-label class="text-h4 text-center" >{{item.index}}</q-item-label>
        </q-item-section>

        <q-item-section class="col-2 text-center">
          <q-item-label class="q-mt-sm text-body1">{{item.title}}</q-item-label>
        </q-item-section>

        <q-item-section >
          <q-item-label lines="2" class="text-center">
            <span class="text-body1">{{item.rem}}</span>
          </q-item-label>
        </q-item-section>

        <q-item-section >
          <q-item-label lines="2" class="text-center">
            <span class="text-body1">{{item.total}}</span>
          </q-item-label>
        </q-item-section>

        <q-item-section >
          <q-item-label lines="2" class="text-center">
            <span class="text-body1">{{item.rate}}</span>
          </q-item-label>
        </q-item-section>

        <q-item-section >
          <q-item-label lines="2" class="text-center">
            <span class="text-body1">{{item.days_rem}}</span>
          </q-item-label>
        </q-item-section>
      </q-item>
    </q-list>
</template>

<script>
export default {
  name: 'TodoTask',
  data() {
    return {
      items: [
        {
          index: '1',
          title: 'DBMS Vids',
          rem: '80',
          total: '165',
          rate: '2',
          days_rem: '20'
        },
        {
          index: '2',
          title: 'CN Vids',
          rem: '20',
          total: '180',
          rate: '2',
          days_rem: '20'
        }
      ]
    }
  },
  
}
</script>
