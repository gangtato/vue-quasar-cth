<template>
  <q-page>
     <div class="row q-gutter">
       <div class="col-6">
         <section class="q-ma-md">
          <q-img src="https://aclc.kpk.go.id/content/view?filename=71a7f856-478f-4b29-90f5-0d6db1cc1ae7"/>
         </section>
         </div>
       <div class="col-6">
         <section class="q-ma-md">
           <div class="text-h5">Pelaksanaan RCC Penyuluh Antikorupsi Jenjang Muda Batch I</div>

          <div class="q-item q-item-type row no-wrap q-mt-md q-item--dense">
              <div class="q-item__section column q-item__section--avatar q-item__section--side justify-center">
                <q-btn size="sm" outline icon="calendar_today" round color="primary">
                  <q-popup-proxy cover transition-show="scale" transition-hide="scale">
                    <q-date
                    subtitle="Tanggal Kegiatan: 22 Februari 2022 - 24 Februari 2022"
                    :events="events" />
                  </q-popup-proxy>
                </q-btn>
              </div>

              <div class="q-item__section column q-item__section--main justify-center">
                <p class="pa">22 Februari 2022 - 24 Februari 2022,</p>
                <p class="pa">08:00 - selesai</p>
              </div>
          </div>

          <div class="q-item q-item-type row no-wrap q-mt-md q-item--dense">
              <div class="q-item__section column q-item__section--avatar q-item__section--side justify-center">
                <q-icon name="location_on" color="primary" size="sm"/>
              </div>

              <div class="q-item__section column q-item__section--main justify-center">
                 Asesmen Jarak Jauh (via zoom), Jakarta
              </div>
          </div>

          <p class="q-mt-md"><b>PENDAFTARAN RCC PENYULUH ANTIKORUPSI JENJANG MUDA BATCH I</b></p>
          <p>
            Pendaftaran  RCC Penyuluh Antikorupsi 2022 dapat dilakukan melalui Aplikasi Aksesku Interaksi pada tautan :
            <a href="http://akseskuinteraksi.id">http://akseskuinteraksi.id</a>
          </p>
          <p class="text-italic">Jenjang yang dibuka adalah: Jenjang Muda</p>
          <div>
            <p class="pa"><b>Waktu Pelaksanaan : 22-24 Februari 2022</b></p>
            <p class="pa">Tempat            : Asesmen Jarak Jauh (AJJ) TUK LSP KPK via zoom</p>
            <p class="pa">Jenjang          : Muda</p>
            <p class="pa">Tanggal Mulai Pendaftaran     : 17 Januari 2022</p>
            <p class="pa">Batas Akhir Pendaftaran        : 26 Januari 2022</p>
          </div>

          <div class="q-gutter-md q-mt-md">
            <q-btn outline color="primary" label="Detail Program" tag="a" :href="detailProgram" />
            <q-btn color="primary" style="color: white" label="Registrasi Sekarang" tag="a" :href="registrasiSekarang" />
          </div>
         </section>

       </div>
     </div>
  </q-page>
</template>

<script>
import { ref, defineComponent } from 'vue';

export default defineComponent({
  name: 'PageIndex',
  setup () {
    const events = ref([ '2022/02/22','2022/02/23','2022/02/24' ])
    const detailProgram = ref("https://aclc.kpk.go.id/program/sertifikasi/sertifikasi-penyuluh-antikorupsi/tentang")
    const registrasiSekarang = ref("http://akseskuinteraksi.id/")
    window.document.title = 'Pelaksanaan RCC Penyuluh Antikorupsi Jenjang Muda Batch I'
    return {
      events,
      detailProgram,
      registrasiSekarang
    }
  }
})
</script>
<style scoped>
.images{
  max-width: 600px;
  width: 100%;
}
.pa{
  padding: 0;
  margin: 0;
}
.italic{
  font-style: italic;
}
</style>