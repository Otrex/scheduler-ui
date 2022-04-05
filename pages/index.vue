<template>
  <div class="layout bg-F8F9FD">
    <div class="flex">
      <Sidebar @checked="(checked)=> sidebarChecked = checked"/>

      <div :class=" sidebarChecked ? 'main_checked': 'main'">
        <div class="pl-12 pr-6">
          <div class="md:flex md:items-center md:justify-between pt-10 pb-10 -mx-2">
            <div class="py-5 md:py-0">
              <a class="breadcrumbs px-2">{{$route.params.detail || 'Projects'}}</a>
              <span class="px-2 c-#ececec">></span>
              <a class="breadcrumbs c-#ececec px-2">OSE Banking App</a>
            </div>


            <div class="flex items-center py-5 md:py-0">
              <div class="flex relative px-5">
                <svg xmlns="http://www.w3.org/2000/svg" height="24px" viewBox="0 0 24 24" width="24px" fill="#000000"><path d="M0 0h24v24H0z" fill="none"/><path d="M21 6h-2v9H6v2c0 .55.45 1 1 1h11l4 4V7c0-.55-.45-1-1-1zm-4 6V3c0-.55-.45-1-1-1H3c-.55 0-1 .45-1 1v14l4-4h10c.55 0 1-.45 1-1z"/></svg>
              </div>
                
              <div class="px-8">
                <svg xmlns="http://www.w3.org/2000/svg" height="24px" viewBox="0 0 24 24" width="24px" fill="#000000"><path d="M12 22c1.1 0 2-.9 2-2h-4c0 1.1.89 2 2 2zm6-6v-5c0-3.07-1.64-5.64-4.5-6.32V4c0-.83-.67-1.5-1.5-1.5s-1.5.67-1.5 1.5v.68C7.63 5.36 6 7.92 6 11v5l-2 2v1h16v-1l-2-2z"/></svg>
              </div>
  
              <div class="px-10">
                <div class="flex items-center -mx-2">
                  <div class="px-2">
                    <span class="inline-block p-4 border-radius-50p bg-#1e212c">
                      <img src="http://placehold.it/" />
                    </span>
                  </div>
                  <div class="c-#1e212c px-2"> RonasIT</div>
                  <div class="px-2">
                    <svg xmlns="http://www.w3.org/2000/svg" height="24px" viewBox="0 0 24 24" width="24px" fill="#000000"><path d="M0 0h24v24H0V0z" fill="none"/><path d="M7.41 8.59L12 13.17l4.59-4.58L18 10l-6 6-6-6 1.41-1.41z"/></svg>
                  </div>
                </div>
              </div>
            </div>
          </div>

          <div class="md:flex md:items-center md:justify-between py-0">
            <div class="py-5 md:py-0">
              <h2 class="pb-2">GSE Banking app</h2>
              <div class="flex items-center -mx-2">
                <span class="px-2 c-#ececec small-p3">56%</span> 
                <div class="w-full px-2">
                  <div class="h-1 bg-#131e3a-opac w-6/12 border-radius-16px">
                    <div class="bg-#1d5cfc p-0.5 border-radius-16px w-6/12"></div>
                  </div>
                </div>
              </div>
            </div>


            <div class="flex items-center justify-between -mx-5 py-5 md:py-0">
              <div class="px-5">
                <button class="flex items-center justify-between border-2px-dashed-#ececec p-3 border-radius-16px">
                  <div class="flex relative px-3">
                    <svg class="c-#ececec" xmlns="http://www.w3.org/2000/svg" height="24px" viewBox="0 0 24 24" width="24px" fill="#000000"><path d="M0 0h24v24H0z" fill="none"/><path d="M19 13h-6v6h-2v-6H5v-2h6V5h2v6h6v2z"/></svg>
                  </div>
                  <span class="c-#ececec"> invite </span>
                </button>
              </div>

              <div class="px-5">
                <div class="flex items-center">
                  <img src="https://picsum.photos/30/30" class="inline-block h-auto w-auto border-radius-50p bg-#12a8f6 -mr-2" />
                  <img src="https://picsum.photos/30/30" class="inline-block h-auto w-auto border-radius-50p bg-#12a8f6 -mr-2" />
                  <img src="https://picsum.photos/30/30" class="inline-block h-auto w-auto border-radius-50p bg-#12a8f6 -mr-2" />
                  <span class="inline-flex items-center justify-center w-8 h-8 border-radius-50p bg-#1e212c">
                    <span class="c-white inline-block small-p2">+15</span>
                  </span>
                </div>
              </div>
            </div>
          </div>




          <div class="md:flex md:items-center md:justify-between py-10">
            <div class="flex items-center -mx-2 py-5 md:py-0">
              <h6 class="px-2">{{presentMonth}} {{presentYear}}</h6>
              <div class="flex items-center px-2">
                <span class="px-2 c-#ececec"> b </span>
                <span class="px-2 c-#ececec"> > </span>
              </div>
            </div>


            <div class="flex items-center justify-between -mx-5 py-5 md:py-0">
              <div class="px-5">
                <svg xmlns="http://www.w3.org/2000/svg" height="24px" viewBox="0 0 24 24" width="24px" fill="#000000"><path d="M0 0h24v24H0z" fill="none"/><path d="M15.5 14h-.79l-.28-.27C15.41 12.59 16 11.11 16 9.5 16 5.91 13.09 3 9.5 3S3 5.91 3 9.5 5.91 16 9.5 16c1.61 0 3.09-.59 4.23-1.57l.27.28v.79l5 4.99L20.49 19l-4.99-5zm-6 0C7.01 14 5 11.99 5 9.5S7.01 5 9.5 5 14 7.01 14 9.5 11.99 14 9.5 14z"/></svg>
              </div>

              <div class="px-5">
                <select class="w-full block p-3 border-1px-solid-#ececec p-3 border-radius-25px" style="min-width: 170px;">
                  <option value="month">month</option>
                </select>
              </div>
            </div>
          </div>

          <div class="pt-0 pb-5 relative">
            <div class="flex overflow-x-auto w-full">   
              <div class="">
                <div class="relative overflow-auto">
                  <div class="flex py-10">
                    <div v-for="(curr, i) in allDaysInMonth" :key="i"  class="flex px-5 py-2 -mx-1" :class="{['bg-#1d5cfc border-radius-16px p-3 c-white']: curr.presentDate, ['pl-0']: i=== 0, ['pr-0']: i=== allDaysInMonth.length - 1}"> 
                      <p class="c-#ececec text-uppercase px-1">
                        {{curr.day.split('')[0]}}
                      </p>
                      <p class="px-1">
                        {{curr.date}}
                      </p>
                    </div>
                  </div>

                  <div class="grid chart-lines px-5 py-2 -mx-1 my-2" :style="{ gridTemplateColumns: 'repeat(' + allDaysInMonth.length + ',' + '1fr)'}">
                    <span 
                      class="border-right-1px-solid-#ececec"
                      :class="{ ['flex justify-center']: days.presentDate== true}" 
                      v-for="(days, i) in allDaysInMonth" :key="i"
                    >
                    </span>
                    <!-- <span v-for="(days, i) in allDaysInMonth" :key="i" :class="{ ['hidden']: checkCurrentDate(days)}">
                      <span v-if="checkCurrentDate(curr)"  :class="{ ['border-right-1px-#12a8f6']: checkCurrentDate(days)}"></span>
                    </span> -->
                  </div>

                  <div v-for="(staff, i) in staffs" :key="i" class="flex relative">

                    <div class="absolute md:w-4/12 z-100 my-4">
                      <div class="md:w-full bg-white flex items-center justify-between p-5 border-1px-solid-#ececec border-radius-16px">
                        <div class="flex items-center -mx-2">
                          <div class="px-2">
                            <img src="https://picsum.photos/50/50" class="inline-block h-auto w-auto border-radius-50p bg-#12a8f6 -mr-2" />
                          </div>

                          <div class="px-2">
                            <h6>{{staff.name}}</h6>
                            <p class="c-#ececec small-p2">{{staff.role}}</p>
                          </div>
                        </div>

                        <div class="cursor-pointer">
                          <svg xmlns="http://www.w3.org/2000/svg" height="24px" viewBox="0 0 24 24" width="24px" fill="#000000"><path d="M0 0h24v24H0z" fill="none"/><path d="M12 8c1.1 0 2-.9 2-2s-.9-2-2-2-2 .9-2 2 .9 2 2 2zm0 2c-1.1 0-2 .9-2 2s.9 2 2 2 2-.9 2-2-.9-2-2-2zm0 6c-1.1 0-2 .9-2 2s.9 2 2 2 2-.9 2-2-.9-2-2-2z"/></svg>
                        </div>
                      </div>
                    </div>


                    <div class="relative w-10/12 z-10 my-4">
                      <div class="w-full grid" :style="{ gridTemplateColumns: 'repeat(' + allDaysInMonth.length + ',' + '1fr)'}">
                        <div :style="generateGraph(staff)" class="overflow-hidden border-radius-50px border relative">

                          <div class="flex justify-between items-center">
                            <div class="flex overflow-hidden items-center border-radius-50px -mx-2 p-3 z-100">
                              <div class="px-2 z-100">
                                <div class="outer-circle"></div> 
                              </div>
                              <div class="px-2">
                                <p class="small-p3 c-white">
                                  {{staff.work.name}}
                                </p>
                              </div>
                            </div>

                            <span class="text-right z-100 pr-3" :style="`color: ${staff.work.bgColor}`">
                            {{staff.work.progress + '%'}}
                            </span>
                          </div>

                          <div 
                            class="absolute top-0 left-0 right-0 bottom-0 flex overflow-hidden items-center border-radius-50px p-3" 
                            :style="progressBar(staff)"
                          ></div>
                         
                        </div>
                      </div>
                    </div>

                  </div>
                </div>
              </div>
            </div>

          </div>

        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: 'IndexPage',
  data(){
    return{
      sidebarChecked: null,
      today: new Date(),
      presentMonth: null,
      presentYear: null,
      selectedMonth: null,
      months: ['January', 'February', 'March', 'April', 'May', 'June', 'July', 'August', 'September', 'October', 'November', 'December'],
      week: ['Sunday', 'Monday', 'Tuesday', 'Wednesday', 'Thursday', 'Friday', 'Saturday'],
      allDaysInMonth: [],
      staffs: [
        { name: 'Finna A', role: 'UI Designer', work: { name: '', bgColor: '', progress: 0, startDate: '', endDate:''} },
        { name: 'Emma F', role: 'UI Designer', work: { name: '', bgColor: '', progress: 0, startDate: '', endDate:''}},
        { name: 'Alex B', role: 'UI Designer', work: { name: '', bgColor: '', progress: 0, startDate: '', endDate:''}},
        { name: 'Cody D', role: 'UI Designer', work: { name: '', bgColor: '', progress: 0, startDate: '', endDate:''}},
        { name: 'Samantha G', role: 'Senoir UX/UI Designer', work: { name: '', bgColor: '', progress: 0, startDate: '', endDate:''}},
        { name: 'Erik F', role: 'UI Designer', work: { name: '', bgColor: '', progress: 0, startDate: '', endDate:''}},
        { name: 'Anna S', role: 'UI Designer', work: { name: '', bgColor: '', progress: 0, startDate: '', endDate:''}},
        { name: 'Enma S', role: 'UI Designer', work: { name: '', bgColor: '', progress: 0, startDate: '', endDate:''}},
        { name: 'Rock D', role: 'UI Designer', work: { name: '', bgColor: '', progress: 0, startDate: '', endDate:''}},
        { name: 'Harvey S', role: 'UI Designer', work: { name: '', bgColor: '', progress: 0, startDate: '', endDate:''}},
      ],
      workItems: [
        { 
          name: 'flow Swift Transfer', 
          bgColor: '#1d5cfc', 
          opacityBg: 'rgba(29,92,252, 0.1)',
          progress: 0,
          startDate: '', 
          endDate: ''
        },
        { 
          name: 'end flow Swift Transfer', 
          bgColor: '#fd7e2e', 
          opacityBg: 'rgba(253,126,46, 0.1)',
          progress: 0,
          startDate: '', 
          endDate: ''
        },
        { 
          name: 'User Profile', 
          bgColor: '#f9d018', 
          opacityBg: 'rgba(249,208,24, 0.1)',
          progress: 0,
          startDate: '', 
          endDate: ''
        },
        { 
          name: 'Transfers by Phone Number', 
          bgColor: '#1bd3fc', 
          opacityBg: 'rgba(27,211,252, 0.1)',
          progress: 0,
          startDate: '', 
          endDate: ''
        },
        { 
          name: 'ChatBot', 
          bgColor: '#131e3a', 
          opacityBg: 'rgba(19,30,58, 0.1)',
          progress: 0,
          startDate: '', 
          endDate: ''
        },
        { 
          name: 'Transaction Analytics', 
          bgColor: 'red', 
          opacityBg: 'rgba(255, 0, 0, 0.1)',
          progress: 0,
          startDate: '', 
          endDate: ''
        },
        { 
          name: 'Settings', 
          bgColor: 'green', 
          opacityBg: 'rgba(0,255, 0, 0.1)',
          progress: 0,
          startDate: '', 
          endDate: ''
        },
        { 
          name: 'Create Storypoint', 
          bgColor: 'orange', 
          opacityBg: 'rgba(255, 69, 0, 0.1)',
          progress: 0,
          startDate: '', 
          endDate: ''
        },
        { 
          name: 'backend testing', 
          bgColor: 'fuchsia', 
          opacityBg: 'rgba(249, 132, 239, 0.1)',
          progress: 0,
          startDate: '', 
          endDate: ''
        },
        { 
          name: 'deployment', 
          bgColor: 'indigo', 
          opacityBg: 'rgba(75,0,130, 0.1)',
          progress: 0,
          startDate: '', 
          endDate: ''
        },
      ]
    }
  },

  created(){},

  mounted(){
    this.showCalendar(new Date().getMonth(), new Date().getFullYear());
    this.assignEventsToWorkers();
    console.log(this.$route.path);
    setInterval(() => {
      console.log('timeout')
      this.staffs.forEach((curr)=>{
        if(curr.work.progress >= 100){
          curr.work.progress = 100
        }else{
          curr.work.progress = curr.work.progress + this.randomInteger(10, 10)
        }   
        console.log(this.staffs);
        return curr;
      })
    }, 15000);
  },

  methods:{
    checkCurrentDate(curr){
      if(curr && curr.presentDate) return curr.presentDate;
    },
    checkProgress(staff){
      if(staff && staff.work && staff.work.progress) return staff.work.progress > 10;
    },
    progressBar(staff){
      if(staff && staff.work && staff.work.progress) return `background: ${staff.work.bgColor}; width: ${staff.work.progress}%`
    },

    generateGraph(staff){
      if(staff && staff.work && staff.work.startDate && staff.work.endDate) return `background: ${staff.work.opacityBg}; grid-column: ${staff.work.startDate.getDate() - 10}/${staff.work.endDate.getDate() - 8}`
    },

    checkdayAndTaskDate(staff, curr){
      console.log('val', staff.work.startDate.getDate(), curr.date)
      return staff.work.startDate.getDate() === curr.date || staff.work.endDate.getDate() === curr.date
    },

    randomDate(start, end) {
      var today = new Date()
      var date = new Date(today.getFullYear(), today.getMonth(), start + Math.random() * (end - start));
      // var new Date()
      console.log('d start', start, end)
      console.log('date', date)
      return date;

      
      // var startDate = start.getTime();
      // var endDate = end.getTime();
      // var spaces = (endDate - startDate);
      // var timestamp = Math.round(Math.random() * spaces);
      // timestamp += startDate;
      // return new Date(timestamp);
    },

    daysInMonth(iMonth, iYear) { 
      return 32 - new Date(iYear, iMonth, 32).getDate();
    },

    showCalendar(month, year) {
      let firstDay = (new Date(year, month)).getDay();
      this.presentMonth = this.months[month];
      this.presentYear = year;
      this.selectedMonth = month;
      console.log('firstday', firstDay)
      const totalDaysInMonth = this.daysInMonth(month, year)
      const today = new Date();
      for(let i = today.getDate() - 10; i < today.getDate() + 8; i++){
        let d = new Date(today.getFullYear(), today.getMonth(), i);
        const day = { date: d.getDate(), day: this.week[d.getDay()], presentDate: today.getDate() === d.getDate() }
        this.allDaysInMonth.push(day);
      }
    },

    assignEventsToWorkers(){
      this.workItems.forEach((element, idx) => {
        element.startDate = this.randomDate(new Date().getDate(), new Date().getDate() - ((Math.floor(Math.random() * 18))+ 1));
        element.endDate = this.randomDate(new Date().getDate(), new Date().getDate() + ((Math.floor(Math.random() * 6))+ 1));
        return element;
      });
      
      this.staffs.forEach((element, idx) => {
        element.work = Array.from(new Set(this.shuffle(this.workItems)))[idx];
        return element;
      });
    },
    
    shuffle(array) {
      let currentIndex = array.length, randomIndex;
      while (currentIndex != 0) {
        randomIndex = Math.floor(Math.random() * currentIndex);
        currentIndex--;
        [array[currentIndex], array[randomIndex]] = [array[randomIndex], array[currentIndex]];
      }
      return array;
    },

    randomInteger(min, max) {
      return Math.floor(Math.random() * (max - min + 1)) + min;
    }

  }
}
</script>


<style scoped>
.outer-circle {
	background: #fff;
	border-radius: 50%;
	height: 10px;
	width:10px;
  position: relative;
  box-shadow: 0 0 0 10px rgba(255,255,255, 0.2);
  margin: 10px;
}
  
.chart-lines {
  position: absolute;
  height: 100%;
  width: 100%;
  background-color: transparent;
}

.chart-lines > span {
  display: block;
}

</style>