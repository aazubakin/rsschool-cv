# Aleksandr Zubakin

### Contact Info: 
   * tel: +7 (912) 836-31-36
   * email: eldoson@yandex.ru
### Summary:
My goal is to become professional developer. In now time I see myself as web-developer. Focused on JavaScript and I very like to programming in that language. Ten years ago when I was a student, I thought that programming for special people and I will never work as developer. Since, I worked in many places and never as developer. But to become a developer it is my dream, that starting to be true right now. I'm not going to stop to realize it.

### Skills:
HTML5, CSS, JavaScript, PHP, MySQL

### Code examples (LATEST):
```JavaScript
//Observer task, subscribe for events
module.exports = {

    /**
     * @param {String} event
     * @param {Object} subscriber
     * @param {Function} handler
     */
    on: function (event, subscriber, handler) {
        if (this[event] === undefined) {
            this[event] = [];
        }
        this[event].push({ subscriber: subscriber, handler: handler });
        return this;
    },

    /**
     * @param {String} event
     * @param {Object} subscriber
     */
    off: function (event, subscriber) {
        if (this[event] !== undefined) {
            this[event] = this[event].filter(element => element.subscriber != subscriber);
        }
        return this;
    },

    /**
     * @param {String} event
     */
    emit: function (event) {
        if (this[event] !== undefined) {
            for (var i = 0; i < this[event].length; i++) {
                this[event][i].handler.call(this[event][i].subscriber);
            }
        }

        return this;
    }
};

```
### Experience: 
* Social network "Distance": https://aazubakin.github.io/distance/ ([source](https://github.com/aazubakin/distance))
* Advertisement's site like avito.ru: https://aazubakin.github.io/awito-js/([source](https://github.com/aazubakin/awito-js))
* Poster to the film "Ghostbusters": https://aazubakin.github.io/ghostbuster-poster/([source](https://github.com/aazubakin/ghostbuster-poster))

### Education:
* 2018 - Chelyabinsk State University, Economics.
* 2011 - Shadrinks State University, Computer Science.

Courses: 
* September 2020 - Michigan State University, Building Web Applications in PHP, [sertificate](https://www.coursera.org/account/accomplishments/verify/MUGRDMRST5R7)
* September 2020 - MPhTI, Basic HTML and CSS, [sertificate](https://www.coursera.org/account/accomplishments/verify/MPSN3MW3BEKH)
* August 2020 - MPhTI, JavaScript, part 1: basic and functions, [sertificate](https://www.coursera.org/account/accomplishments/verify/NBNBNNYDMEBA)

### English:
Participated in the program "Work and Travel" as student. I'm studied english in Truman College of Chicago. My second job in career was Schlumberger as IT support, often I had to answer on english language by phone.