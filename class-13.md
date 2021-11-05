## Local Storage for Web Applications ##

1. Cookies can be used for persistent local storage of small amounts of data
2. What we really want is
   - a lot of storage space
   - on the client
   - that persists beyond a page refresh
   - and isn’t transmitted to the server

3. Check for HTML5 Storage

  - function supports_html5_storage() {
      try {
        return 'localStorage' in window && window['localStorage'] !== null;
      } catch (e) {
        return false;
      }
    }

  Instead of writing this function yourself, you can use Modernizr to detect support for HTML5 Storage.

  - if (Modernizr.localstorage) {
      // window.localStorage is available!
    } else {
      // no native support for HTML5 storage :(
      // maybe try dojox.storage or a third-party solution
    }

4. Actual working code in 4 browsers

  - openDatabase('documents', '1.0', 'Local document storage', 5*1024*1024, function (db) {
      db.changeVersion('', '1.0', function (t) {
        t.executeSql('CREATE TABLE docids (id, name)');
      }, error);
    });