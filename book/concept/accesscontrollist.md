# AccessControlList

:thumbsup:

IL faut une bonne idée ici .)

Genre efficace et complète&#x20;

Première idée si je vois cet  ACL et qu'il est nul c'est que j'ai droit car j'ai l'accès a l'asset parent qui ma donné accès cet asset.&#x20;

Sinon l'acl est non nul&#x20;

ZZZ Ce qui suit n'est pas bon (il n'y a pas de groupes).&#x20;

```javascript

class User {
    constructor(name, role) {
        this.name = name;
        this.role = role;
    }
}

class ACL {
    constructor() {
        this.permissions = {
            'read': ['user', 'admin'],
            'write': ['admin'],
            'delete': ['admin']
        };
    }
    addPermission(action, role) {
    if (this.permissions[action]) {
        if (!this.permissions[action].includes(role)) {
            this.permissions[action].push(role);
        }
    } else {
        this.permissions[action] = [role];
    }
    }
    checkPermission(user, action) {
        if (this.permissions[action].includes(user.role)) {
            return true;
        }
        return false;
    }
    toJSON() {
        return JSON.stringify(this.permissions);
    }

    static fromJSON(json) {
        let acl = new ACL();
        acl.permissions = JSON.parse(json);
        return acl;
    }
}

let user1 = new User('Alice', 'user');
let user2 = new User('Bob', 'admin');
let acl = new ACL();

console.log(acl.checkPermission(user1, 'read')); // true
console.log(acl.checkPermission(user1, 'write')); // false
console.log(acl.checkPermission(user2, 'write')); // true

// Convertir l'ACL en JSON
let json = acl.toJSON();

// Sauvegarder json dans la base de données...

// Récupérer json de la base de données...

// Convertir le JSON en ACL
let aclFromDB = ACL.fromJSON(json);
```
